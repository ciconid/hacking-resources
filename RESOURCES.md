# RESOURCES

# - TOOLS

## + BurpSuite
- ### Extensions
        - Para Miner
        - Content type converter
        - Turbo intruder

## + DOMAIN/SUBDOMAIN ENUMERATION
- ### subfinder
- ### amass
- ### assetfinder
- ### findomain
- ### sublister
- ### ffuf
    https://github.com/ffuf/ffuf

    - OUTPUT:   
        `ffuf -o <filename> -of <output-format>`
        > Choose csv as output format and then use awk to filter the first column of the results

        `ffuf -o ffuf-results.csv -of csv` 
        
        `awk -F ',' '{print $1}' ffuf-results.csv `
        >awk's flag -F is used to identify the comma as the column separator

        > I chose csv because the default option (json) has a lot of info that I currently don't need. I only wanted the names of the identified directories (or whatever parameter we are fuzzing)
- ### altdns
       generates alternative domain names by doing permutations of a given list of words

        NahamSec uses shuffledns to validate the domains, but I think httpx could also work

## + HTTP tools
- ### httpx
    [github.com/projectdiscovery/httpx](https://github.com/projectdiscovery/httpx)

        Useful flags:
            -sc, -status-code
            -cl, -content-length
            -title
            -td, -tech-detect




## + Content Discovery / Directory Bruteforcing
	
	feroxbuster
	dirbust
	gobuster
	ffuf

## + Web crawlers

- ### katana
    https://github.com/projectdiscovery/katana

    
## + HASH
https://crackstation.net/

## + VULNERABILITY SCANNER
- ### nuclei

- ### katana


<br />
<br />

# - CHECKLISTS
### My checklists
    TO DO:

    OWASP top 10 vulnerabilities
    - IDOR
    - XXS
    - SQLi
    - Authentication
    
### links
https://github.com/crackallcode/Bug-Bounty-Checklist

https://github.com/sehno/Bug-bounty/blob/master/bugbounty_checklist.md#authentication

https://github.com/KathanP19/HowToHunt/tree/master

https://gowthams.gitbook.io/bughunter-handbook/checklists



# READING MATERIALS
### Recon
https://dhiyaneshgeek.github.io/bug/bounty/2020/02/06/recon-with-me/


<br />
<br />

# NOT YET TESTED/TRIED
Google Admin Toolbox