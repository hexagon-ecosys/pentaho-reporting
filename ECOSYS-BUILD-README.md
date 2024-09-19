# Gradle Build README for EcoSys #

1. Build https://github.com/hexagon-ecosys/pentaho-commons-database first
2. Then build 'libraries' under this repo in the following order -
   1. flute
   2. libbase
   3. libswing
   4. libserializer
   5. librepository
   6. libformula
   7. libformat
   8. libpixie
   9. libloader
   10. libxml
   11. libfonts
   12. libdocbundle
3. Finally build 'core'

## NOTES ##
* The latest branch for both repos is 202409-1 (indicating that master was merged in Sep 2024)
* **Pentaho has changed licensing to BSL 1.1 as of Sep 3 2024, which essentially means we cannot refresh this going forward**
* Look at the Git log to see which revision from master was last merged in to this branch
* Run the unit tests for everything you build -
  * There are a few failures in 'core' that have to do with a test DB login failure ... ignore them
  * There are a few minor failures in 'libformat' where the word 'at' goes missing ... ignore them
