[avalanche](../README.md) › [API-EVM-Credentials](../modules/api_evm_credentials.md) › [SECPCredential](api_evm_credentials.secpcredential.md)

# Class: SECPCredential

## Hierarchy

  ↳ [Credential](common_signature.credential.md)

  ↳ **SECPCredential**

## Index

### Constructors

* [constructor](api_evm_credentials.secpcredential.md#constructor)

### Properties

* [_codecID](api_evm_credentials.secpcredential.md#protected-_codecid)
* [_typeID](api_evm_credentials.secpcredential.md#protected-_typeid)
* [_typeName](api_evm_credentials.secpcredential.md#protected-_typename)
* [sigArray](api_evm_credentials.secpcredential.md#protected-sigarray)

### Methods

* [addSignature](api_evm_credentials.secpcredential.md#addsignature)
* [clone](api_evm_credentials.secpcredential.md#clone)
* [create](api_evm_credentials.secpcredential.md#create)
* [deserialize](api_evm_credentials.secpcredential.md#deserialize)
* [fromBuffer](api_evm_credentials.secpcredential.md#frombuffer)
* [getCodecID](api_evm_credentials.secpcredential.md#getcodecid)
* [getCredentialID](api_evm_credentials.secpcredential.md#getcredentialid)
* [getTypeID](api_evm_credentials.secpcredential.md#gettypeid)
* [getTypeName](api_evm_credentials.secpcredential.md#gettypename)
* [select](api_evm_credentials.secpcredential.md#select)
* [serialize](api_evm_credentials.secpcredential.md#serialize)
* [setCodecID](api_evm_credentials.secpcredential.md#setcodecid)
* [toBuffer](api_evm_credentials.secpcredential.md#tobuffer)

## Constructors

###  constructor

\+ **new SECPCredential**(`sigarray`: Array‹[Signature](common_signature.signature.md)›): *[SECPCredential](api_evm_credentials.secpcredential.md)*

*Inherited from [Credential](common_signature.credential.md).[constructor](common_signature.credential.md#constructor)*

*Defined in [src/common/credentials.ts:163](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/common/credentials.ts#L163)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`sigarray` | Array‹[Signature](common_signature.signature.md)› | undefined |

**Returns:** *[SECPCredential](api_evm_credentials.secpcredential.md)*

## Properties

### `Protected` _codecID

• **_codecID**: *number* = undefined

*Inherited from [Serializable](utils_serialization.serializable.md).[_codecID](utils_serialization.serializable.md#protected-_codecid)*

*Defined in [src/utils/serialization.ts:42](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/utils/serialization.ts#L42)*

___

### `Protected` _typeID

• **_typeID**: *number* = EVMConstants.SECPCREDENTIAL

*Overrides [Credential](common_signature.credential.md).[_typeID](common_signature.credential.md#protected-_typeid)*

*Defined in [src/apis/evm/credentials.ts:27](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/apis/evm/credentials.ts#L27)*

___

### `Protected` _typeName

• **_typeName**: *string* = "SECPCredential"

*Overrides [Credential](common_signature.credential.md).[_typeName](common_signature.credential.md#protected-_typename)*

*Defined in [src/apis/evm/credentials.ts:26](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/apis/evm/credentials.ts#L26)*

___

### `Protected` sigArray

• **sigArray**: *Array‹[Signature](common_signature.signature.md)›* = []

*Inherited from [Credential](common_signature.credential.md).[sigArray](common_signature.credential.md#protected-sigarray)*

*Defined in [src/common/credentials.ts:121](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/common/credentials.ts#L121)*

## Methods

###  addSignature

▸ **addSignature**(`sig`: [Signature](common_signature.signature.md)): *number*

*Inherited from [Credential](common_signature.credential.md).[addSignature](common_signature.credential.md#addsignature)*

*Defined in [src/common/credentials.ts:129](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/common/credentials.ts#L129)*

Adds a signature to the credentials and returns the index off the added signature.

**Parameters:**

Name | Type |
------ | ------ |
`sig` | [Signature](common_signature.signature.md) |

**Returns:** *number*

___

###  clone

▸ **clone**(): *this*

*Overrides [Credential](common_signature.credential.md).[clone](common_signature.credential.md#abstract-clone)*

*Defined in [src/apis/evm/credentials.ts:35](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/apis/evm/credentials.ts#L35)*

**Returns:** *this*

___

###  create

▸ **create**(...`args`: any[]): *this*

*Overrides [Credential](common_signature.credential.md).[create](common_signature.credential.md#abstract-create)*

*Defined in [src/apis/evm/credentials.ts:41](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/apis/evm/credentials.ts#L41)*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  deserialize

▸ **deserialize**(`fields`: object, `encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *void*

*Inherited from [Credential](common_signature.credential.md).[deserialize](common_signature.credential.md#deserialize)*

*Overrides [Serializable](utils_serialization.serializable.md).[deserialize](utils_serialization.serializable.md#deserialize)*

*Defined in [src/common/credentials.ts:112](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/common/credentials.ts#L112)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`fields` | object | - |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *void*

___

###  fromBuffer

▸ **fromBuffer**(`bytes`: any, `offset`: number): *number*

*Inherited from [Credential](common_signature.credential.md).[fromBuffer](common_signature.credential.md#frombuffer)*

*Defined in [src/common/credentials.ts:134](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/common/credentials.ts#L134)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`bytes` | any | - |
`offset` | number | 0 |

**Returns:** *number*

___

###  getCodecID

▸ **getCodecID**(): *number*

*Inherited from [Serializable](utils_serialization.serializable.md).[getCodecID](utils_serialization.serializable.md#getcodecid)*

*Defined in [src/utils/serialization.ts:61](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/utils/serialization.ts#L61)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getCredentialID

▸ **getCredentialID**(): *number*

*Overrides [Credential](common_signature.credential.md).[getCredentialID](common_signature.credential.md#abstract-getcredentialid)*

*Defined in [src/apis/evm/credentials.ts:31](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/apis/evm/credentials.ts#L31)*

**Returns:** *number*

___

###  getTypeID

▸ **getTypeID**(): *number*

*Inherited from [Serializable](utils_serialization.serializable.md).[getTypeID](utils_serialization.serializable.md#gettypeid)*

*Defined in [src/utils/serialization.ts:54](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/utils/serialization.ts#L54)*

Used in serialization. Optional. TypeID is a number for the typeID of object being output.

**Returns:** *number*

___

###  getTypeName

▸ **getTypeName**(): *string*

*Inherited from [Serializable](utils_serialization.serializable.md).[getTypeName](utils_serialization.serializable.md#gettypename)*

*Defined in [src/utils/serialization.ts:47](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/utils/serialization.ts#L47)*

Used in serialization. TypeName is a string name for the type of object being output.

**Returns:** *string*

___

###  select

▸ **select**(`id`: number, ...`args`: any[]): *[Credential](common_signature.credential.md)*

*Overrides [Credential](common_signature.credential.md).[select](common_signature.credential.md#abstract-select)*

*Defined in [src/apis/evm/credentials.ts:45](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/apis/evm/credentials.ts#L45)*

**Parameters:**

Name | Type |
------ | ------ |
`id` | number |
`...args` | any[] |

**Returns:** *[Credential](common_signature.credential.md)*

___

###  serialize

▸ **serialize**(`encoding`: [SerializedEncoding](../modules/utils_serialization.md#serializedencoding)): *object*

*Inherited from [Credential](common_signature.credential.md).[serialize](common_signature.credential.md#serialize)*

*Overrides [Serializable](utils_serialization.serializable.md).[serialize](utils_serialization.serializable.md#serialize)*

*Defined in [src/common/credentials.ts:105](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/common/credentials.ts#L105)*

**Parameters:**

Name | Type | Default |
------ | ------ | ------ |
`encoding` | [SerializedEncoding](../modules/utils_serialization.md#serializedencoding) | "hex" |

**Returns:** *object*

___

###  setCodecID

▸ **setCodecID**(`codecID`: number): *void*

*Inherited from [Credential](common_signature.credential.md).[setCodecID](common_signature.credential.md#setcodecid)*

*Defined in [src/common/credentials.ts:124](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/common/credentials.ts#L124)*

**Parameters:**

Name | Type |
------ | ------ |
`codecID` | number |

**Returns:** *void*

___

###  toBuffer

▸ **toBuffer**(): *Buffer*

*Inherited from [Credential](common_signature.credential.md).[toBuffer](common_signature.credential.md#tobuffer)*

*Defined in [src/common/credentials.ts:146](https://github.com/ava-labs/avalanchejs/blob/cfff19f/src/common/credentials.ts#L146)*

**Returns:** *Buffer*