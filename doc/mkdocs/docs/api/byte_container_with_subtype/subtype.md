# byte_container_with_subtype::subtype

```cpp
constexpr subtype_type subtype() const noexcept;
```

Returns the numerical subtype of the value if it has a subtype. If it does not have a subtype, this function will return
`subtype_type(-1)` as a sentinel value.

## Return value

the numerical subtype of the binary value, or `subtype_type(-1)` if no subtype is set

## Complexity

Constant.

## Exception safety

No-throw guarantee: this function never throws exceptions.

## Version history

- Added in version 3.8.0
- Fixed return value to properly return `subtype_type(-1)` as documented in version 3.10.0.