# CSV on the Web validator service

[CSV on the Web](https://www.w3.org/2013/csvw/wiki/Main_Page) is a set of W3C Recommendations from 2015.
It can be used for describing CSV files published on the Web using a JSON-LD descriptor containing the CSV table schema and other metadata.

The problem is that there is no decent validator implementation that could be used by data publishers to verify that their CSV files and JSON-LD descriptors are correct.

There is the [CSVW Implementation Report](http://w3c.github.io/csvw/publishing-snapshots/PR-earl/earl.html) indicating that there are currently 2 compliant implementations, [csvlint](https://github.com/theodi/csvlint.rb) and [RDF::Tabular](http://rubygems.org/gems/rdf-tabular). Both of these tools are Ruby based and, unfortunately, they do not work reliably, suffer from various bugs and are not developed anymore. In addition, csvlint has its online version [csvlint.io](http://csvlint.io/), which only supports [JSON Table Schema](https://frictionlessdata.io/specs/table-schema/) deprecated by the CSV on the Web Recommendation, which causes confusion among data publishers.

If there is a better implementation available, please let us know. We are not aware of any, and therefore will try to implement our own.
