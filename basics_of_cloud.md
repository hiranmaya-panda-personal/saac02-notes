# Basics of Cloud Computing

## IAM Access Keys
Access Key ID
Secret Key

AWS CLI v2
aws --version
aws configure --profile <profilename>
aws s3 ls

## Cloud Computing
1. On-demand self-service
2. Broad network access
3. Resource pooling
4. Rapid elasticity
5. Measured service

## Types of Cloud
1. Public Cloud = using 1 Public Cloud
2. Private Cloud = using on-premises *real* cloud
3. Multi-Cloud = using more than 1 public cloud
4. Hybrid Cloud = Public & Private Clouds

Hybrid Cloud != public cloud + legacy on-premises infrastructure (= Hybrid networking)

## Service Models
Infrastructure stack.

Based on the "Unit of consumption", the type of service model is defined.
Ex: EC2 instance's UoC is the OS, Netflix's UoC is the application & nothing else.

On-premises vs DC Hosted - Traditionally used. Datacentre hosting vendor provided Facilities for consumption.

Cloud service Models
1. IaaS - UoC is O/S
2. PaaS (esp. used by the Developers) - UoC is Runtime
3. SaaS - UoC is the application

## Other necessary topics
### YAML
YAML ain't markup language!
Used in AWS' CloudFormation service.

Human readable - data serialization language.

key: value format

*List Examples:*
```yaml key: ["value 1","value 2","value 3"]```

OR

yaml key:
 - value 1
 - "value 2"
 - 'value 3'
 
Indentation is critical in YAML to verify the correct structure of items within a List.

*YAML Dictionary:* 
Unordered set of key-value pairs.

parent_key:
  - key1: value1
    key2: ["value2", "value3"]
  - key3: "value 4"
    key4: value5
    key5: 1.2

### JSON
JavaScript Object Notation!
- Lightweight data-interchange format.
- Easy for humans to read/write. Easy for machines to parse & generate.
- Doesn't care about indentation unlike YAML.
Used in AWS's CloudFormation & other services, ex - Policy documentation.

*JSON object*
- Unordered set of key-value pairs. Enclosed by { & }.
- Ex - {key1: value1, key2: value2}
- Analogus to YAML's dictionary.

*JSON Array*
- Ordered collection of values. Enclosed by [ & ].
- Ex - [value1, value2, value3]
- Analogus to YAML's Lists.

JSON objects can be nested for complex structures.

Note the *values* in JSON & YAML can be strings, arrays, floats, integers, true, false, null.



