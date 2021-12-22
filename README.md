# precursor: GoldenEye version 2.1 by Jan Seidl

EagleEye is only a tool for SECURITY TESTING PURPOSES!

EagleEye is an HTTP DoS Test Tool.

Attack Vector exploited: HTTP Keep Alive + NoCache

Warning: don't try with .edu and .gov

## Usage

      git clone https://github.com/lucthienphong1120/EagleEye.git
      cd EagleEye
      python3 eagleeye.py --help

## Options:
```
        python3 eagleeye.py <url> <options>
        Options            Description                                      Default
        -u, --useragents   Type of user-agents to generate                  (default: randomly generated)
                           (see in http://www.useragentstring.com/)
        -w, --workers      Number of concurrent workers to attack           (default: 50)
        -s, --sockets      Number of concurrent sockets                     (default: 100)
        -m, --method       HTTP Method to use                               (default: get)
                           (get/post/random)
        -d, --debug        Enable Debug Mode (more verbose output)          (default: False)
                           (True/False)
        -n, --nosslcheck   Do not verify SSL Certificate                    (default: True)
                           (True/False)
        -h, --help         Shows this help
        
        
        Example: python3 eagleeye.py https://example.com -w 1000 -s 1000 -m post
```

Check website monitoring in https://check-host.net/


## Utilities
   
* Added randomly created user agents (still RFC compliant).
* Added external user-agent list support.
* http://www.useragentstring.com/
* Increased worker and socket capacity.
* Changed from threading to multiprocessing.
* Improved randomness of referers.
* Added Debug Mode.
* Added support for not verifying SSL Certificates.


## License
This software is distributed under the GNU General Public License version 3 (GPLv3)

## LEGAL NOTICE
THIS SOFTWARE IS PROVIDED FOR EDUCATIONAL USE ONLY!
WARNING: DON'T TRY WITH .EDU AND .GOV
IF YOU ENGAGE IN ANY ILLEGAL ACTIVITY THE AUTHOR DOES NOT TAKE ANY RESPONSIBILITY FOR IT. 
BY USING THIS SOFTWARE YOU AGREE WITH THESE TERMS.
