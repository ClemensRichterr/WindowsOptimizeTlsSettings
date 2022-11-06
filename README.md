# Windows - Optimize Tls Settings

## Story

I built these reg files because I noticed that the configuration in Windows is set rather weakly by default, which is of course clear because Microsoft has to ensure broad compatibility. Nevertheless, some of the cipher suites used are insecure or no longer up to date. The same applies to the SSL/TLS versions etc., which can be set with the reg files. If one of the two REG files causes something to no longer work, you can import the backup (bak.reg). One of the REG files is based on the BSI document TR-02102-2, the other is a little stricter and removes the cipher suites with the CBC mode.

## Usage

 1. Copy the reg files to the Windows computer you want to configure.
 2. Install (Double click on the file) one of the two TLS REG XXX.reg files

- **BSI**: based on the BSI document TR-02102-2.
- **STRICT**: based on the BSI document TR-02102-2 + removes the cipher suites with the CBC mode.

### Hints

If something should no longer work after the installation, simply install the **bak.reg** file.

## Note of Thanks

Thanks for [IIS Crypto](https://www.nartac.com/Products/IISCrypto/) ✌, because without it these reg files would not have been possible!
