[**@tevm/solc**](../README.md)

***

[@tevm/solc](../globals.md) / SolcStorageLayoutInplaceType

# Interface: SolcStorageLayoutInplaceType

Defined in: [solcTypes.ts:513](https://github.com/evmts/tevm-monorepo/blob/main/bundler-packages/solc/src/solcTypes.ts#L513)

A storage layout type that is laid out contiguously in storage.

## Extends

- [`SolcStorageLayoutTypeBase`](SolcStorageLayoutTypeBase.md)

## Extended by

- [`SolcStorageLayoutStructType`](SolcStorageLayoutStructType.md)

## Properties

### encoding

> **encoding**: `"inplace"`

Defined in: [solcTypes.ts:514](https://github.com/evmts/tevm-monorepo/blob/main/bundler-packages/solc/src/solcTypes.ts#L514)

How the data is encoded in storage

- inplace: data is laid out contiguously in storage
- mapping: keccak-256 hash-based method
- dynamic_array: keccak-256 hash-based method
- bytes: single slot or keccak-256 hash-based depending on the data size

#### Overrides

[`SolcStorageLayoutTypeBase`](SolcStorageLayoutTypeBase.md).[`encoding`](SolcStorageLayoutTypeBase.md#encoding)

***

### label

> **label**: `string`

Defined in: [solcTypes.ts:501](https://github.com/evmts/tevm-monorepo/blob/main/bundler-packages/solc/src/solcTypes.ts#L501)

The canonical type name

#### Inherited from

[`SolcStorageLayoutTypeBase`](SolcStorageLayoutTypeBase.md).[`label`](SolcStorageLayoutTypeBase.md#label)

***

### numberOfBytes

> **numberOfBytes**: `string`

Defined in: [solcTypes.ts:507](https://github.com/evmts/tevm-monorepo/blob/main/bundler-packages/solc/src/solcTypes.ts#L507)

The number of used bytes (as a decimal string)

Note: if numberOfBytes > 32 this means that more than one slot is used

#### Inherited from

[`SolcStorageLayoutTypeBase`](SolcStorageLayoutTypeBase.md).[`numberOfBytes`](SolcStorageLayoutTypeBase.md#numberofbytes)
