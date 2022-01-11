# Github Actions Tutorial

## Yaml
- Yet another Markup Language
- An alternative to simplified JSON files
- Used in CI/CD operations
- A cleaner way to read and space-sensitive (Indentations) specific.

## JSON to YAML
### Objects

- JSON representation\
    {
        "key": "value"
    }
- YAML representation\
key:value

### Arrays
- JSON representation\
    {\
        &emsp;"key": [1,2,3,4]\
    }
- YAML representation\
key: [1,2,3,4] or\
key:
    - 1
    - 2
    - 3
    - 4

### Array of Objects
- JSON representation\
    {\
        &emsp;"keys": [\
            &emsp;&emsp;{\
                &emsp;&emsp;&emsp; "key1": "value1",\
                &emsp;&emsp;&emsp; "key2": "value2"\
            &emsp;&emsp;},\
            &emsp;&emsp;{\
                &emsp;&emsp;&emsp; "key3": "value3"\
            &emsp;&emsp;}\
        &emsp;]\
    }
- YAML representation\
keys:
    - key1: value1
      key2: value2 # As key2 is under the same object of the first element no, '-'
    - key3: value3 

### Multiline Strings
- JSON representation\
    {\
        "key": "Sample\nLine\nSeperated\nwith\nnewline\ncharacters"\
    }
- YAML representation\
key: | # Added a pipe to have multiline strings formatted\
    &emsp;Sample\
    &emsp;Line\
    &emsp;Seperated\
    &emsp;with\
    &emsp;newline\
    &emsp;characters