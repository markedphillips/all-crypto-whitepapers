# allcryptowhitepapers.com parser and pdf downloader

https://github.com/markedphillips/all-crypto-whitepapers/

Blockchain paper downloader. And the whitepapers it downloaded.

### Development

The main file is ./wget_pdfs.sh. It basically uses a .list file of URLs for various blockchain/coins and downloads the associated PDFs copies them into a whitepapers directory. There are some test files for a regex machine learning tool. The resulting regex to parse a webpage for the links.

This project was inspired by https://github.com/a-r-d/all-crypto-whitepapers, but instead of looping through a csv which had the name of the coin and link to the associated paper, I was super lazy. The idea of hunting for actual links to whitepaper pdfs was actually the point for a machine.

So this repo points towards a site purporting to have all the whitepapers, it crawls the site and traverses ALL the links, when it finds a whitepaper it saves it, otherwise it throws away the html file or whatever it is. The included code took about 28 hours on a 100MB/s connection crawling to search through 2419 whitepaper descriptions finally collecting 272 papers. The papers are included here so you don't have to do the same work. This is by far the largest collection of whitepapers easilly accesible via git clone https://github.com/markedphillips/all-crypto-whitepapers.

### Todo

I could have renamed the files better to map to the purported name of the coin. I also could have OCR'd the files and exported a text file for those that need to search for common key ideas faster. These are things I'll probably do locally and push up later.
