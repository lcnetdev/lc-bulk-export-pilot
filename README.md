Please create any issues with the new bulk download pilot here.


LCNAF - Pilot

We are testing a new bulk export process for LCSH and would like to hear any feedback from anyone who uses the bulk downloads. The new bulk files can be found http://id.loc.gov/download/ with the titles LC Subject Headings (LCSH) \*NEW Pilot\*
```
New:
 - New compacted JSON-LD  serialization
 - The JSON-LD and XML files are now newline delimited meaning each line in the file is a completely self-contained record
 - There are void files for each download with the date the export was created, title, description and MD5 hash of the unzipped download.
 - The N-Triple file has records separators now as comments, each group of triples start with “# Start of n12345678”
 - Increased updated frequency.
            
The same:
 - The new LCNAF export will contain the same data as before, but is slightly more verbose.
 - It is available in MADSRDF, SKOS and both combined MADSRDF and SKOS in all serializations.
            
Thinking of removing:
 - The current XML dump is one large XML file, the new XML is each record as RDF XML on its own individual line. The current XML file could be used for bulk loading into a triple store, but the current and future NT file could be used in the same way. Is anyone using the current XML dump file for bulk loading?
 - The Turtle serialization
```

---


LCSH - Pilot

We are testing a new bulk export process for LCSH and would like to hear any feedback from anyone who uses the bulk downloads. The new bulk files can be found http://id.loc.gov/download/ with the titles LC Subject Headings (LCSH) \*NEW Pilot\*
```
New:
- New compacted JSON-LD  serialization
- The JSON-LD and XML files are now newline delimited meaning each line in the file is a completely self-contained record
- There are void files for each download with the date the export was created, title, description and MD5 hash of the unzipped download.
- The N-Triple file has records separators now as comments, each group of triples start with “# Start of sh12345678”
- Increased updated frequency, should be updated when new LCSH updates are released monthly.

The same:
- The new LCSH export will contain the same data as before, including broader and narrower relationship but is slightly more verbose.
- It is available in MADSRDF, SKOS and both combined MADSRDF and SKOS in all serializations.

Thinking of removing:
- The current XML dump is one large XML file, the new XML is each record as RDF XML on its own individual line. The current XML file could be used for bulk loading into a triple store, but the current and future NT file could be used in the same way. Is anyone using the current XML dump file for bulk loading?
- The Turtle serialization

```
Samples: 
The first 10 records for MADSRDF & SKOS in all serializations:
https://gist.github.com/thisismattmiller/0691f815478a5dc337e2e140becfc549

