# REQUIREMENTS #
� Nmap v6.47 or higher (also tested with v6.49)
� Modified nselib (included)



# Setup #
Place the .nse file here:
/usr/share/nmap/scripts/

Place the packet2.lua file here:
/usr/share/nmap/nselib/



# Example usage #
nmap -sS -PN -n -T4 -p 80 --script=�SYNfulKnock� 10.1.1.1/24

FLAG EXPLANATION:
-sS = SYN scan
-PN = Don�t perform host discovery
-n = Don�t perform name resolution
-T4 = Throttle to speed 4
-p = port number
--script = script to execute
optional: --scriptargs=�reportclean=1� Shows the seq and ack for clean
devices too