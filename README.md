# Response

- [1. Property `Response > id`](#id)
- [2. Property `Response > status`](#status)
- [3. Property `Response > value`](#value)
  - [3.1. Property `Response > value > anyOf > item 0`](#value_anyOf_i0)
    - [3.1.1. Response > value > anyOf > item 0 > item 0 items](#value_anyOf_i0_items)
  - [3.2. Property `Response > value > anyOf > item 1`](#value_anyOf_i1)
    - [3.2.1. Response > value > anyOf > item 1 > item 1 items](#value_anyOf_i1_items)
  - [3.3. Property `Response > value > anyOf > item 2`](#value_anyOf_i2)
    - [3.3.1. Response > value > anyOf > item 2 > item 2 items](#value_anyOf_i2_items)
  - [3.4. Property `Response > value > anyOf > item 3`](#value_anyOf_i3)
  - [3.5. Property `Response > value > anyOf > item 4`](#value_anyOf_i4)
  - [3.6. Property `Response > value > anyOf > item 5`](#value_anyOf_i5)
  - [3.7. Property `Response > value > anyOf > item 6`](#value_anyOf_i6)
- [4. Property `Response > subform`](#subform)
- [5. Property `Response > code`](#code)
- [6. Property `Response > score`](#score)

**Title:** Response

|                           |                  |
| ------------------------- | ---------------- |
| **Type**                  | `object`         |
| **Required**              | No               |
| **Additional properties** | Any type allowed |

**Description:** Data structure produced by verona players

| Property               | Pattern | Type             | Deprecated | Definition | Title/Description                                                                                                                     |
| ---------------------- | ------- | ---------------- | ---------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| + [id](#id )           | No      | string           | No         | -          | Identifier for the data source (variable)                                                                                             |
| + [status](#status )   | No      | enum (of string) | No         | -          | Status as stage in the workflow of creating and coding a variable's value                                                             |
| + [value](#value )     | No      | Combination      | No         | -          | -                                                                                                                                     |
| - [subform](#subform ) | No      | string           | No         | -          | If variables i. e. data source ids are not unique in the unit, 'subform' can specify the sub object related to the specific variable. |
| - [code](#code )       | No      | integer          | No         | -          | Code representing the category of the value after coding process.                                                                     |
| - [score](#score )     | No      | integer          | No         | -          | This value represents the result evaluation of the code after coding process.                                                         |

## <a name="id"></a>1. Property `Response > id`

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | Yes      |

**Description:** Identifier for the data source (variable)

**Examples:**

```json
"IE7873"
```

```json
"UHZ654"
```

| Restrictions                      |                                                                                                             |
| --------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| **Must match regular expression** | ```^[0-9a-zA-Z_]+$``` [Test](https://regex101.com/?regex=%5E%5B0-9a-zA-Z_%5D%2B%24&testString=%22IE7873%22) |

## <a name="status"></a>2. Property `Response > status`

|              |                    |
| ------------ | ------------------ |
| **Type**     | `enum (of string)` |
| **Required** | Yes                |

**Description:** Status as stage in the workflow of creating and coding a variable's value

Must be one of:
* "UNSET"
* "NOT_REACHED"
* "DISPLAYED"
* "VALUE_CHANGED"
* "DERIVE_ERROR"
* "CODING_COMPLETE"
* "NO_CODING"
* "INVALID"
* "CODING_INCOMPLETE"
* "CODING_ERROR"
* "PARTLY_DISPLAYED"
* "DERIVE_PENDING"
* "INTENDED_INCOMPLETE"

## <a name="value"></a>3. Property `Response > value`

|                           |                  |
| ------------------------- | ---------------- |
| **Type**                  | `combining`      |
| **Required**              | Yes              |
| **Additional properties** | Any type allowed |

| Any of(Option)            |
| ------------------------- |
| [item 0](#value_anyOf_i0) |
| [item 1](#value_anyOf_i1) |
| [item 2](#value_anyOf_i2) |
| [item 3](#value_anyOf_i3) |
| [item 4](#value_anyOf_i4) |
| [item 5](#value_anyOf_i5) |
| [item 6](#value_anyOf_i6) |

### <a name="value_anyOf_i0"></a>3.1. Property `Response > value > anyOf > item 0`

|              |         |
| ------------ | ------- |
| **Type**     | `array` |
| **Required** | No      |

|                      | Array restrictions |
| -------------------- | ------------------ |
| **Min items**        | N/A                |
| **Max items**        | N/A                |
| **Items unicity**    | False              |
| **Additional items** | False              |
| **Tuple validation** | See below          |

| Each item of this array must be       | Description |
| ------------------------------------- | ----------- |
| [item 0 items](#value_anyOf_i0_items) | -           |

#### <a name="value_anyOf_i0_items"></a>3.1.1. Response > value > anyOf > item 0 > item 0 items

|              |                  |
| ------------ | ---------------- |
| **Type**     | `string or null` |
| **Required** | No               |

### <a name="value_anyOf_i1"></a>3.2. Property `Response > value > anyOf > item 1`

|              |         |
| ------------ | ------- |
| **Type**     | `array` |
| **Required** | No      |

|                      | Array restrictions |
| -------------------- | ------------------ |
| **Min items**        | N/A                |
| **Max items**        | N/A                |
| **Items unicity**    | False              |
| **Additional items** | False              |
| **Tuple validation** | See below          |

| Each item of this array must be       | Description |
| ------------------------------------- | ----------- |
| [item 1 items](#value_anyOf_i1_items) | -           |

#### <a name="value_anyOf_i1_items"></a>3.2.1. Response > value > anyOf > item 1 > item 1 items

|              |                  |
| ------------ | ---------------- |
| **Type**     | `number or null` |
| **Required** | No               |

### <a name="value_anyOf_i2"></a>3.3. Property `Response > value > anyOf > item 2`

|              |         |
| ------------ | ------- |
| **Type**     | `array` |
| **Required** | No      |

|                      | Array restrictions |
| -------------------- | ------------------ |
| **Min items**        | N/A                |
| **Max items**        | N/A                |
| **Items unicity**    | False              |
| **Additional items** | False              |
| **Tuple validation** | See below          |

| Each item of this array must be       | Description |
| ------------------------------------- | ----------- |
| [item 2 items](#value_anyOf_i2_items) | -           |

#### <a name="value_anyOf_i2_items"></a>3.3.1. Response > value > anyOf > item 2 > item 2 items

|              |                   |
| ------------ | ----------------- |
| **Type**     | `boolean or null` |
| **Required** | No                |

### <a name="value_anyOf_i3"></a>3.4. Property `Response > value > anyOf > item 3`

|              |          |
| ------------ | -------- |
| **Type**     | `number` |
| **Required** | No       |

### <a name="value_anyOf_i4"></a>3.5. Property `Response > value > anyOf > item 4`

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | No       |

### <a name="value_anyOf_i5"></a>3.6. Property `Response > value > anyOf > item 5`

|              |        |
| ------------ | ------ |
| **Type**     | `null` |
| **Required** | No     |

### <a name="value_anyOf_i6"></a>3.7. Property `Response > value > anyOf > item 6`

|              |           |
| ------------ | --------- |
| **Type**     | `boolean` |
| **Required** | No        |

## <a name="subform"></a>4. Property `Response > subform`

|              |          |
| ------------ | -------- |
| **Type**     | `string` |
| **Required** | No       |

**Description:** If variables i. e. data source ids are not unique in the unit, 'subform' can specify the sub object related to the specific variable.

## <a name="code"></a>5. Property `Response > code`

|              |           |
| ------------ | --------- |
| **Type**     | `integer` |
| **Required** | No        |

**Description:** Code representing the category of the value after coding process.

## <a name="score"></a>6. Property `Response > score`

|              |           |
| ------------ | --------- |
| **Type**     | `integer` |
| **Required** | No        |

**Description:** This value represents the result evaluation of the code after coding process.

----------------------------------------------------------------------------------------------------------------------------
Generated using [json-schema-for-humans](https://github.com/coveooss/json-schema-for-humans) on 2025-02-26 at 10:28:17 +0000
