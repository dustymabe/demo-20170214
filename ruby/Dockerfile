FROM dustymabe/fedora-min
MAINTAINER Dusty Mabe <dusty@dustymabe.com>
RUN microdnf install ruby rubygem-sinatra && microdnf clean all
COPY hello_ruby.rb /hello_ruby.rb
EXPOSE 4567
ENTRYPOINT ["/hello_ruby.rb", "-o", "0.0.0.0", "-p", "4567"]
