# subenum
Enumerate subdomain using crtsh and certspotter

### usage

Add `crtspotter` and `crtsh` to `PATH` 
```
crtspotter example.com
crtsh example.com
```
- To find subdomains of domians in `domians.txt`
```sh
for i in `<domains.txt`; do echo "scanning : $i"; crtsh $1 | tee -a all.txt; certspotter $i | tee -a all.txt; sleep 1; done;
```
# TODO
Add more tools and automate whole process
