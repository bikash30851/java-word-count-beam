# java-word-count-beam
java word count using apache beam

### WordCount quickstart for Java

Link to commands

https://beam.apache.org/get-started/quickstart-java/

1. Generate a Maven example project that builds against the latest Beam release:

```
mvn archetype:generate `
  -D archetypeGroupId=org.apache.beam `
  -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
  -D archetypeVersion=2.42.0 `
  -D groupId=org.example `
  -D artifactId=word-count-beam `
  -D version="0.1" `
  -D package=org.apache.beam.examples `
  -D interactiveMode=false
   
```

2. Change into word-count-beam:

```
cd .\word-count-beam
   
```

3. List the example pipelines:
```
dir .\src\main\java\org\apache\beam\examples
   
```

## Running WordCount using Maven

```
mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount `
 -D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner
```

## Inspecting the results

```
ls counts*
   
```
```
more counts*
```

[Word Count Running](runningbeam.png) 
[First Name](firstname.png) 
[Last_Name](lastname.png) 
