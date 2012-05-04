twdel
=====

Twitter history remover

Purpose
-------
This program is made to clear the history of an account of Twitter.
Twdel removes all the "statuses" of an authenticated account, as far as the API allows.

Requirements
------------
 - perlbrew + cpanm
 - Perl >= 5.10

3. Howto Install
You of course must download this application, and type the following command to install requirements

    $ cpanm Net::Twitter Config::Pit LWP::Protocol::https

Usage
-----
### Authentication ###
First you must authenticate the application by executing the following command:

    $ ./authenticate

This command will ask you to open a URL necessary to allow this application to access your account.
The authentication information will be stored under `~/.pit` (this does not include your Twitter password).
### Removal ###
And then you can remove your history by the following command:

    $ ./twdel
    
This will connect to your account and removes your statuses from newer to older.

