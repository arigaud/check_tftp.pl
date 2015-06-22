# check_tftp.pl
TFTP Monitor for Nagios

Needs Net::TFTP

   Usage:
   OA_EXT_check_tftp.pl [-d] -H hostname -f file1,file2,... [-T <timeout>]
   [-s service -p port -r retry -t ftp_timeout -m mode -b blocksize]
   OA_EXT_check_tftp.pl [-h | --help]
   OA_EXT_check_tftp.pl [-v | --version]

   Options:
        --hostname
           Server's hostname
        --timeout
           Global timeout
        --filename
           Filenames (separated by comma)
        --debug
           Debug perl TFTP on
        --port
           Port to send data to (default: 69)
        --retry
           Maximum number of retries (default: 5)
        --tftp_timeout
           Timeout in seconds before retry (default: 5)
        --mode
           Mode to transfer data in, "octet" or "netascii" (default: netascii)
        --blocksize
           Negotiate size of blocks to use in the transfer (default: 512)
        --service
           select one of the following keywords:
           get  (Get REMOTE_FILE from the server)
           put  (Put a file to the server as REMOTE_FILE)
