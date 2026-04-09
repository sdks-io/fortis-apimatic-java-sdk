
# Field Configuration

field_configuration

## Structure

`FieldConfiguration`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `CssMini` | `Boolean` | Optional | CSS Mini | Boolean getCssMini() | setCssMini(Boolean cssMini) |
| `Stack` | [`StackEnum`](../../doc/models/stack-enum.md) | Optional | Stack | StackEnum getStack() | setStack(StackEnum stack) |
| `Header` | [`Header`](../../doc/models/header.md) | Optional | Header | Header getHeader() | setHeader(Header header) |
| `Body` | [`Body`](../../doc/models/body.md) | Optional | Body | Body getBody() | setBody(Body body) |
| `Footer` | [`Footer`](../../doc/models/footer.md) | Optional | Footer | Footer getFooter() | setFooter(Footer footer) |

## Example (as JSON)

```json
{
  "css_mini": true,
  "stack": "vertical",
  "header": {
    "settings": {
      "enabled": false,
      "columns": 202.28,
      "rows": 235.78
    },
    "fields": [
      {
        "id": "id8",
        "label": "label8",
        "field_type": "field_type4",
        "position": [
          "position7",
          "position8",
          "position9"
        ],
        "required": false
      }
    ]
  },
  "body": {
    "settings": {
      "enabled": false,
      "columns": 202.28,
      "rows": 235.78
    },
    "fields": [
      {
        "id": "id8",
        "label": "label8",
        "field_type": "field_type4",
        "position": [
          "position7",
          "position8",
          "position9"
        ],
        "required": false
      },
      {
        "id": "id8",
        "label": "label8",
        "field_type": "field_type4",
        "position": [
          "position7",
          "position8",
          "position9"
        ],
        "required": false
      },
      {
        "id": "id8",
        "label": "label8",
        "field_type": "field_type4",
        "position": [
          "position7",
          "position8",
          "position9"
        ],
        "required": false
      }
    ]
  },
  "footer": {
    "settings": {
      "enabled": false,
      "columns": 202.28,
      "rows": 235.78
    },
    "fields": [
      {
        "id": "id8",
        "label": "label8",
        "field_type": "field_type4",
        "position": [
          "position7",
          "position8",
          "position9"
        ],
        "required": false
      },
      {
        "id": "id8",
        "label": "label8",
        "field_type": "field_type4",
        "position": [
          "position7",
          "position8",
          "position9"
        ],
        "required": false
      }
    ]
  }
}
```

