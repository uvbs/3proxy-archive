/*
   3APA3A simpliest proxy server
   (c) 2002 by ZARAZA <3APA3A@security.nnov.ru>

   please read License Agreement

   $Id: Readme,v 1.1.1.1 2003/07/19 11:18:19 vlad Exp $
*/

See http://www.security.nnov.ru/soft/3proxy/howtoe.asp (English)
 or http://www.security.nnov.ru/soft/3proxy/howtor.asp (Russian)
for manual.

3proxy.exe	Combined proxy server may be used as Windows 95/98/NT/2000/XP
		executable or Windows NT/2000/XP service (supports
		installation and removal). It uses config file to read
		it's configuration (see 3proxy.cfg.sample for details).
		--install installs and starts proxy as NT/2000/XP service
		(config file should be located in the same directory)
		--remove removes the service (should be stopped before via
		net stop 3proxy).
		3proxy.exe is all-in-one, it doesn't require all others .exe
		to work.
		See 3proxy.cfg.sample for configuration manual and examples
proxy.exe	HTTP proxy server, binds to port 3128
socks.exe	SOCKS 4/5 proxy server, binds to port 1080
pop3p.exe	POP3 proxy server, binds to port 110. You must specify
		POP3 username as username@target.host.ip[:port]
		port is 110 by default.
		Exmple: in Username configuration for you e-mail reader
		set someuser@pop.somehost.ru, to obtains mail for someuser
		from pop.somehost.ru via proxy.
tcppm.exe	TCP port mapping. Maps some TCP port on local machine to
		TCP port on remote host.
udppm.exe	UDP port mapping. Maps some UDP port on local machine to
		UDP port on remote machine. Only one user simulationeously
		can use UDP mapping, so it cann't be used for public service
		in large networks. It's OK to use it to map to DNS server
		in small network or to map Counter-Strike server for single
		client (you can use few mappings on different ports for
		different clients in last case).
mycrypt.exe	Program to obtain crypted password fro cleartext. Supports
		both MD5/crypt and NT password.
			mycrypt password
		produces NT password
			mycrypt salt password
		produces MD5/crypt password with salt "salt".
dighosts.exe	Utility for building networks list from web page.


Run utility with --help option to obtain command line reference.

Latest version available from http://www.security.nnov.ru/soft
