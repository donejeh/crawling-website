Web Crawler Problem
-----

### Description

Build a command line script that you can call with a URL and it will begin crawling all links on
that website and printing out every link it finds to console.log. 

For example:

If you put in the url https://www.amazon.com it would check the HTML for that website and then
any link it finds, print the link to console.log and try to load the HTML for that page and print
any more links it finds on the new page.

This process continues until all links are exhausted. Only links within the same domain should
be visited and printed out.

### Setup Instructions

First, install dependencies by running npm install from the program's root directory
```
$ npm install
```

Install package globally to have access from command line anywhere
```
$ npm install -g .
```

Run the program from the command line with the crawler command
```
$ crawl
```

### Usage

Usage: crawl [[arguments] url] [options]

Options:
   --help ------------- Show help

argument:
   -n [Integer] ------ Set Number of workers (Optional)

Samples:
```
Crawl https://www.amazon.com
```
```
Crawl -n 4 https://www.amazon.com
```

### Testing

For testing, run npm test 
```
$ npm test
```
To check coverage, npm run test-coverage
```
$ npm run test-coverage
```

### Requirements

node v10.5 and above (Required for worker-threads)