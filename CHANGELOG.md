## 2.0.5
 - Support signature_version option for v4 S3 keys
## 2.0.4
 - Remove the `Time.now` stub in the spec, it was conflicting with other test when running inside the default plugins test #63
 - Make the spec run faster by adjusting the values of time rotation test.
## 2.0.3
 - Update deps for logstash 2.0
## 2.0.2
 - Fixes an issue when tags were defined #39
## 2.0.0
 - Plugins were updated to follow the new shutdown semantic, this mainly allows Logstash to instruct input plugins to terminate gracefully,
   instead of using Thread.raise on the plugins' threads. Ref: https://github.com/elastic/logstash/pull/3895
 - Dependency on logstash-core update to 2.0

# 1.0.1
- Fix a synchronization issue when doing file rotation and checking the size of the current file
- Fix an issue with synchronization when shutting down the plugin and closing the current temp file
