# allcryptowhitepapers.com parser and pdf downloader

Upon going to the page listing the "3000" blockchain papers, I parse the html and use to create a directory structure with the mirrored files, then find the pdfs. 

### Development

Scripts are in bash and some regex separated in files so I could piece together what I thought would work. This repo orginally was to extend https://github.com/a-r-d/all-crypto-whitepapers but the task of collecting locations for the whitepapers became annoying. After working on the regex, which I hate more than anything, I realized that I could have written the wget function to traverse the site deeper and ditched the whole need for the site parsing. The script throws away coins without whitepapers, but it could be modified to extract the abstract for the coin and the links to any additional information, which after processing 100 whitepapers I decided I wasn't going to read any more than that.