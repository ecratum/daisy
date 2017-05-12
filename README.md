What we are proposing to build is an easy-to use, modularized web interface for *D* that follows the path of RACK on Ruby.

https://rack.github.io/

https://github.com/rack

This would be very appealing to web developers because with this approach, they could easily switch from *Ruby or Python*, then build frameworks on top of **Daisy**. 
This happened in Ruby, when RACK was extracted from the **RubyOnRails** framework.
Also the modularization would give developers easy access to what they exactly need.
Building it could be done based on the patterns in RACK. RACK is very well documented so will be quite easy to pick up.

The core features of this interface could be the following:

- content_type: Setting a content-type header on responses that do not have one. Repo: https://github.com/ecratum/daisy_content-type
- logger: We should be able to log all the events in the daily, we should be able to granulate the results also, we should use and improve the dlang logger class. Repo: https://github.com/ecratum/daisy_logger
- media_type: Setting media type (type/subtype) portion of the content_type header without any media type parameters. Repo: https://github.com/ecratum/daisy_media-type
- query_parser https://github.com/ecratum/daisy_query-parser
- reloader Repo: https://github.com/ecratum/daisy_reloader
- request: Provides a convenient interface to the Daisy environment. Repo: https://github.com/ecratum/daisy_request
- response: Provides a simple interface for response. Repo: https://github.com/ecratum/daisy_response
- sendfile Repo: https://github.com/ecratum/daisy_sendfile
- server Repo: https://github.com/ecratum/daisy_server

The code in each of these would not very big. It could be easily broken down into small subprojects and be organized into a multi-milestone roadmap.
