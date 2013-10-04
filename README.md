bio-mongo
=========

This project contains demonstration code for MongoDB and Genetics.  

  VCFStore:  Generates a JAR file that converts VCF files to JSON and loads them into MongoDB.
  
    Build:  Install Maven
            Check out this repository
              Optional:  Add your MongoDB info to VCFStore/src/main/resources/loader.properties
              (Default Host: localhost, DB: genome)
            mvn package
    
    Result:  Generates VCFStore/target/VCFLoader.jar
    
    Run: java -jar VCFLoader.jar <FileName>.vcf
      Optional:  Replace filename with a Directory full of VCF Files.
      Optional:  use the -public flag to load public VCF files into a different set of collections.
