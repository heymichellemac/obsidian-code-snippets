<%* 
    const randomEvergreenNotes = []

    app.metadataCache.getCachedFiles().forEach(filename => { // get all filenames in the vault and iterate through all of them, calling a function for each of them
        let { tags } = app.metadataCache.getCache(filename) // get the tags in the  file w/ the given name
        tags = (tags || []).filter(t => t.tag && "#evergreen" === t.tag) // filter out all tags that are not "#evergreen"
        
        if (tags.length > 0) { // list will contain at least one tag for the relevant notes
            randomEvergreenNotes.push(filename.slice(13, filename.length - 3)) // removes first 13 characters (03-evergreen/) then cuts off last three characters from filename, otherwise the links would contain `.md` at the end
        }
    })

    var i = 0
    do {
        const randomIndex = Math.floor(Math.random() * randomEvergreenNotes.length)
        tR += `- [[${randomEvergreenNotes[randomIndex]}]]` + "\r\n"
        i++
    } while (i<5)
%>