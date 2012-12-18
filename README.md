check_openvpn
=============

Extended check_openvpn.pl for checking pfSense OpenVPN

Now you can check your OpenVPN status if the server uses a socket for accessing the management.
Check that your monitoring user, e.g. nagios or icinga, can access the OpenVPN server via ssh by
public key authentication and then you can access the socket to check the OpenVPN state.

Example:

    check_openvpn.pl -H firewall.example.org -s /var/etc/openvpn/server1.sock -C user@example.org


