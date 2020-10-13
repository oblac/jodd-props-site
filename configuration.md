# Configuration

_Props_ behavior can be fine-tuned using the following configuration settings:

### escapeNewLineValue

Specifies the new line string when EOL is escaped. Default value is an empty string, so multi-line values will be joined in single-line value. If this value is set to, e.g., `\n`, multi-line values will be persisted as multi-lines.

### valueTrimLeft

Specifies if values should be trimmed from the left.

### valueTrimRight

Specifies if values should be trimmed from the right.

### ignorePrefixWhitespacesOnNewLine

Defines if the leading whitespaces should be ignored when value is split into the lines \(by escaping EOL\). By default it is set to `true`, so the following multi-line props:

```text
key1=line1\
     line2\
line3
```

will be read as `line1line2line3` \(joined\).

### skipEmptyProps

Flag for skipping empty properties.

### appendDuplicateProps

When set, duplicate props key will not override existing one, but will be appended and separated by comma.

### multilineValues

When enabled \(default\), multi-line values may be written in more convenient way using triple-quote \(like in python\). Everything between triple-quotes is considered as a value, so new line does not need to be escaped.

