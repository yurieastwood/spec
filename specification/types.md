# Types and Data Structures

## Overview

This document outlines some of the common types and data structures defined by OpenFeature and referenced elsewhere in this specification.

### Boolean

A logical true or false, as represented idiomatically in the implementation languages.

### String

A UTF-8 encoded string.

### Number

A numeric value of unspecified type or size. Implementation languages may further differentiate between integers, floating point numbers, and other specific numeric types and provide functionality as idioms dictate.

### Structure

Structured data, presented however is idiomatic in the implementation language, such as JSON or YAML.

### Evaluation Details

A structure containing the following fields:

- flag key (string, required)
- value (boolean | string | number | structure, required)
- error code (string, optional)
- reason (string, optional)
- variant (string, optional)

### Flag Resolution

A structure which contains a subset of the fields defined in the `evaluation details` structure, including:

- value (boolean | string | number | structure, required)
- error code (string, optional)
- reason (string, optional)
- variant (string, optional)

### Evaluation Options

A structure containing the following fields:

- hooks (one or more [hooks](./flag-evaluation/hooks.md), optional)
