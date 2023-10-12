# VALIDATION WITH XSD ( XML SCHEMA DEFINITION )

## To-Do
- Validate ROOT element `project` in `pom.xml` using `xsd` file.
- `project` element should nest 4 elments `modelVersion`, `artifactId`, `groupId`, `version` similar to maven project

## Steps
- Declare a new `schema` in `Project.xsd`
- Define a Composite DataType, also know as `complexType`, `Project` with 4 elements `modelVersion`, `artifactId`, `groupId`, `version`
- Define an ROOT element `project` of complexType(DataType) `Project` 
- Use this schema to validate `pom.xml`

## Note
In this example we are using namespace prefix `xs` for namespace `http://www.w3.org/2001/XMLSchema`