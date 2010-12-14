## Sinatra-Dropbox

A very simple Sinatra app that integrates with the Dropbox API.

Requires the dropbox gem
	
	gem install dropbox

To use it just insert your key and secret
	dropbox_session = Dropbox::Session.new('key', 'secret')

And then insert your callback url
	redirect dropbox_session.authorize_url(:oauth_callback => 'http://localhost:9393')

