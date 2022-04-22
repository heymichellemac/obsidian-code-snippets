<%* 
    const randomEvergreenNotes = []

    app.metadataCache.getCachedFiles().forEach(filename => { // get all filenames in the vault and iterate through all of them, calling a function for each of them
        let { tags } = app.metadataCache.getCache(filename) // get the tags in the  file w/ the given name
        tags = (tags || []).filter(t => t.tag && "#evergreen" === t.tag) // filter out all tags that are not "#evergreen"
        
        if (tags.length > 0) { // list will contain at least one tag for the relevant notes
            randomEvergreenNotes.push(filename.slice(13, filename.length - 3)) // removes first 13 characters (03-evergreen/) then cuts off last three characters from filename, otherwise the links would contain `.md` at the end
        }
    })

     // find Q1
    var randomIndex1 = Math.floor(Math.random() * randomEvergreenNotes.length)

    // run loop until Q2 is different from Q1 
    do {
        randomIndex2 = Math.floor(Math.random() * randomEvergreenNotes.length)
    } while (randomIndex1 === randomIndex2);

    // run loop until Q3 is different from Q2 and Q1
    do {
        randomIndex3 = Math.floor(Math.random() * randomEvergreenNotes.length)
    } while (randomIndex3 === randomIndex2 || randomIndex3 === randomIndex1);

    // display the links
    tR += `- [[${randomEvergreenNotes[randomIndex1]}]]` + "\r\n"
    tR += `- [[${randomEvergreenNotes[randomIndex2]}]]` + "\r\n"
    tR += `- [[${randomEvergreenNotes[randomIndex3]}]]` + "\r\n"
%>