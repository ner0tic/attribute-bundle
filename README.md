# Attribute Bundle
Generic attribute base library bundle.

## Installation
```bash
php composer.json update ner0tic\attribute-bundle
```

## Usage
Basic usage.

```php
// Boolean attribute
$public = new BooleanAttribute(
    'is public', 
    array(
        'default_value' => false
    )
);

// Inputable attribute
$evelation = new InputableAttribute(
    'elevation',
    array(
        'default_value' => 0,
        'value_type'    => 'integer'
    )
);

// Choice attribute
$colors = new ChoiceAttribute(
    'colors',
    array(
        'options' => array(
            new Option(
                'red', 
                array(), 
                new Value(
                    'red',
                    array(),
                    'ff0000'
                )
            ),
            new Option(
                'white',
                array(),
                new Value(
                    'white',
                    array(),
                    'ffffff'
                )
            ),
// inputable option
            new Option(
                'custom',
                array(
                    new InputValue(
                        'colors option custom',
                        array(
                            'value_type' => 'hex',
                            'default_value' => 'ffffff'
                        )
                    )
                )
            )
        )
    )
);
```

### Interfaces
- AttributeInterface
- GroupInterface
- OptionInterface
- ValueInterface

### Models
- Attribute
- Group
- Option
- Value

### Entities
- Attribute
- BooleanAttribute
- ChoiceAttribute
- Group
- InputableAttribute
- InputableChoiceAttribute
- InputValue
- Option
- Value

### Documents
- Attribute
- BooleanAttribute
- ChoiceAttribute
- Group
- InputableAttribute
- InputableChoiceAttribute
- InputValue
- Option
- Value

### Forms
- AttributeForm
- BooleanAttributeForm
- ChoiceAttributeForm
- GroupForm
- InputableAttributeForm
- InputableChoiceAttributeForm
- InputValueForm
- OptionForm
- ValueForm

### Repositories
- AttributeRepository
- GroupRespository
- OptionRepository
- ValueRepository

