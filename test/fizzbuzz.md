test/fizzbuzz.mc AST:
{
| {
| | type: VAR
| | {
| | | type: STRUCT
| | | strctName: FizzbuzzMachine
| | | childrenSz: 1
| | | 
| | | decls:
| | | {
| | | | {
| | | | | type: SCOPE
| | | | },
| | | | {
| | | | | type: VAR
| | | | | varName: outs
| | | | | varType: INT
| | | | | isPtr: 1
| | | | | isStatic: 0
| | | | | isArray: 1
| | | | | arrayLength:
| | | | | {
| | | | | | {
| | | | | | | type: LIT
| | | | | | | type: INT
| | | | | | | val: 5
| | | | | | },
| | | | | },
| | | | },
| | | },
| | },
| },
| {
| | type: FUNC
| | funcType: INT
| | isPtr: 0
| | isStatic: 0
| | funcName: main
| | 
| | scope:
| | {
| | | {
| | | | type: VAR
| | | | varName: c
| | | | varType: INT
| | | | isPtr: 0
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: ASSIGN
| | | | varName:
| | | | {
| | | | | {
| | | | | | type: ID
| | | | | | isPtr: 0
| | | | | | varName: c
| | | | | },
| | | | },
| | | | 
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 0
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: VAR
| | | | varName: endAt
| | | | varType: INT
| | | | isPtr: 0
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: ASSIGN
| | | | varName:
| | | | {
| | | | | {
| | | | | | type: ID
| | | | | | isPtr: 2
| | | | | | varName: endAt
| | | | | },
| | | | },
| | | | 
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 1
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: VAR
| | | | varName: fbm
| | | | varType: CUSTOM 3
| | | | isPtr: 0
| | | | isStatic: 1
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: VAR
| | | | varName: count
| | | | varType: INT
| | | | isPtr: 0
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: ASSIGN
| | | | varName:
| | | | {
| | | | | {
| | | | | | type: ID
| | | | | | isPtr: 0
| | | | | | varName: count
| | | | | },
| | | | },
| | | | 
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 0
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: ASSIGN
| | | | varName:
| | | | {
| | | | | {
| | | | | | type: ID
| | | | | | isPtr: 0
| | | | | | varName: fbm
| | | | | | 
| | | | | | nested:
| | | | | | {
| | | | | | | {
| | | | | | | | type: ID
| | | | | | | | isPtr: 0
| | | | | | | | varName: outs
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | | 
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: CALL
| | | | | | funcName: malloc
| | | | | | 
| | | | | | args:
| | | | | | {
| | | | | | | {
| | | | | | | | type: ID
| | | | | | | | isPtr: 0
| | | | | | | | varName: endAt
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: CALL
| | | | funcName: fizzbuzz
| | | | 
| | | | args:
| | | | {
| | | | | {
| | | | | | type: REF
| | | | | | ptr:
| | | | | | {
| | | | | | | {
| | | | | | | | type: ID
| | | | | | | | isPtr: 0
| | | | | | | | varName: c
| | | | | | | },
| | | | | | },
| | | | | },
| | | | | {
| | | | | | type: ID
| | | | | | isPtr: 0
| | | | | | varName: endAt
| | | | | },
| | | | | {
| | | | | | type: REF
| | | | | | ptr:
| | | | | | {
| | | | | | | {
| | | | | | | | type: ID
| | | | | | | | isPtr: 0
| | | | | | | | varName: fbm
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: RET
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 0
| | | | | },
| | | | },
| | | },
| | },
| },
| {
| | type: FUNC
| | funcType: INT
| | isPtr: 0
| | isStatic: 0
| | funcName: fizzbuzz
| | 
| | parameters:
| | {
| | | {
| | | | type: VAR
| | | | varName: count
| | | | varType: INT
| | | | isPtr: 1
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: VAR
| | | | varName: endAt
| | | | varType: INT
| | | | isPtr: 0
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: VAR
| | | | varName: fbm
| | | | varType: CUSTOM 3
| | | | isPtr: 1
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | },
| | 
| | scope:
| | {
| | | {
| | | | type: COND
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: CALL
| | | | | | funcName: isMultiple
| | | | | | 
| | | | | | args:
| | | | | | {
| | | | | | | {
| | | | | | | | type: DEREF
| | | | | | | | exprsn:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: count
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | | {
| | | | | | | | type: LIT
| | | | | | | | type: INT
| | | | | | | | val: 2
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | | 
| | | | scope:
| | | | {
| | | | | {
| | | | | | type: CALL
| | | | | | funcName: print
| | | | | | 
| | | | | | args:
| | | | | | {
| | | | | | | {
| | | | | | | | type: LIT
| | | | | | | | type: INT
| | | | | | | | val: 1111
| | | | | | | },
| | | | | | },
| | | | | },
| | | | | {
| | | | | | type: ASSIGN
| | | | | | varName:
| | | | | | {
| | | | | | | {
| | | | | | | | type: DEREF
| | | | | | | | exprsn:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: BINARY
| | | | | | | | | | stub: 0
| | | | | | | | | | single: 0
| | | | | | | | | | op (id): +
| | | | | | | | | | 
| | | | | | | | | | left:
| | | | | | | | | | {
| | | | | | | | | | | {
| | | | | | | | | | | | type: ID
| | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | varName: fbm
| | | | | | | | | | | | 
| | | | | | | | | | | | nested:
| | | | | | | | | | | | {
| | | | | | | | | | | | | {
| | | | | | | | | | | | | | type: ID
| | | | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | | | varName: outs
| | | | | | | | | | | | | },
| | | | | | | | | | | | },
| | | | | | | | | | | },
| | | | | | | | | | },
| | | | | | | | | | 
| | | | | | | | | | right:
| | | | | | | | | | {
| | | | | | | | | | | {
| | | | | | | | | | | | type: DEREF
| | | | | | | | | | | | exprsn:
| | | | | | | | | | | | {
| | | | | | | | | | | | | {
| | | | | | | | | | | | | | type: ID
| | | | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | | | varName: count
| | | | | | | | | | | | | },
| | | | | | | | | | | | },
| | | | | | | | | | | },
| | | | | | | | | | },
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | },
| | | | | | 
| | | | | | exprsn:
| | | | | | {
| | | | | | | {
| | | | | | | | type: BINARY
| | | | | | | | stub: 1
| | | | | | | | single: 0
| | | | | | | | op (id): +
| | | | | | | | 
| | | | | | | | left:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: DEREF
| | | | | | | | | | exprsn:
| | | | | | | | | | {
| | | | | | | | | | | {
| | | | | | | | | | | | type: BINARY
| | | | | | | | | | | | stub: 0
| | | | | | | | | | | | single: 0
| | | | | | | | | | | | op (id): +
| | | | | | | | | | | | 
| | | | | | | | | | | | left:
| | | | | | | | | | | | {
| | | | | | | | | | | | | {
| | | | | | | | | | | | | | type: ID
| | | | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | | | varName: fbm
| | | | | | | | | | | | | | 
| | | | | | | | | | | | | | nested:
| | | | | | | | | | | | | | {
| | | | | | | | | | | | | | | {
| | | | | | | | | | | | | | | | type: ID
| | | | | | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | | | | | varName: outs
| | | | | | | | | | | | | | | },
| | | | | | | | | | | | | | },
| | | | | | | | | | | | | },
| | | | | | | | | | | | },
| | | | | | | | | | | | 
| | | | | | | | | | | | right:
| | | | | | | | | | | | {
| | | | | | | | | | | | | {
| | | | | | | | | | | | | | type: DEREF
| | | | | | | | | | | | | | exprsn:
| | | | | | | | | | | | | | {
| | | | | | | | | | | | | | | {
| | | | | | | | | | | | | | | | type: ID
| | | | | | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | | | | | varName: count
| | | | | | | | | | | | | | | },
| | | | | | | | | | | | | | },
| | | | | | | | | | | | | },
| | | | | | | | | | | | },
| | | | | | | | | | | },
| | | | | | | | | | },
| | | | | | | | | },
| | | | | | | | },
| | | | | | | | 
| | | | | | | | right:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: LIT
| | | | | | | | | | type: INT
| | | | | | | | | | val: 1
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: COND
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: CALL
| | | | | | funcName: isMultiple
| | | | | | 
| | | | | | args:
| | | | | | {
| | | | | | | {
| | | | | | | | type: DEREF
| | | | | | | | exprsn:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: count
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | | {
| | | | | | | | type: LIT
| | | | | | | | type: INT
| | | | | | | | val: 3
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | | 
| | | | scope:
| | | | {
| | | | | {
| | | | | | type: CALL
| | | | | | funcName: print
| | | | | | 
| | | | | | args:
| | | | | | {
| | | | | | | {
| | | | | | | | type: LIT
| | | | | | | | type: INT
| | | | | | | | val: 1111
| | | | | | | },
| | | | | | },
| | | | | },
| | | | | {
| | | | | | type: ASSIGN
| | | | | | varName:
| | | | | | {
| | | | | | | {
| | | | | | | | type: DEREF
| | | | | | | | exprsn:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: BINARY
| | | | | | | | | | stub: 0
| | | | | | | | | | single: 0
| | | | | | | | | | op (id): +
| | | | | | | | | | 
| | | | | | | | | | left:
| | | | | | | | | | {
| | | | | | | | | | | {
| | | | | | | | | | | | type: REF
| | | | | | | | | | | | ptr:
| | | | | | | | | | | | {
| | | | | | | | | | | | | {
| | | | | | | | | | | | | | type: ID
| | | | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | | | varName: fbm
| | | | | | | | | | | | | | 
| | | | | | | | | | | | | | nested:
| | | | | | | | | | | | | | {
| | | | | | | | | | | | | | | {
| | | | | | | | | | | | | | | | type: ID
| | | | | | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | | | | | varName: outs
| | | | | | | | | | | | | | | },
| | | | | | | | | | | | | | },
| | | | | | | | | | | | | },
| | | | | | | | | | | | },
| | | | | | | | | | | },
| | | | | | | | | | },
| | | | | | | | | | 
| | | | | | | | | | right:
| | | | | | | | | | {
| | | | | | | | | | | {
| | | | | | | | | | | | type: DEREF
| | | | | | | | | | | | exprsn:
| | | | | | | | | | | | {
| | | | | | | | | | | | | {
| | | | | | | | | | | | | | type: ID
| | | | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | | | varName: count
| | | | | | | | | | | | | },
| | | | | | | | | | | | },
| | | | | | | | | | | },
| | | | | | | | | | },
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | },
| | | | | | 
| | | | | | exprsn:
| | | | | | {
| | | | | | | {
| | | | | | | | type: BINARY
| | | | | | | | stub: 1
| | | | | | | | single: 0
| | | | | | | | op (id): +
| | | | | | | | 
| | | | | | | | left:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: DEREF
| | | | | | | | | | exprsn:
| | | | | | | | | | {
| | | | | | | | | | | {
| | | | | | | | | | | | type: BINARY
| | | | | | | | | | | | stub: 0
| | | | | | | | | | | | single: 0
| | | | | | | | | | | | op (id): +
| | | | | | | | | | | | 
| | | | | | | | | | | | left:
| | | | | | | | | | | | {
| | | | | | | | | | | | | {
| | | | | | | | | | | | | | type: REF
| | | | | | | | | | | | | | ptr:
| | | | | | | | | | | | | | {
| | | | | | | | | | | | | | | {
| | | | | | | | | | | | | | | | type: ID
| | | | | | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | | | | | varName: fbm
| | | | | | | | | | | | | | | | 
| | | | | | | | | | | | | | | | nested:
| | | | | | | | | | | | | | | | {
| | | | | | | | | | | | | | | | | {
| | | | | | | | | | | | | | | | | | type: ID
| | | | | | | | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | | | | | | | varName: outs
| | | | | | | | | | | | | | | | | },
| | | | | | | | | | | | | | | | },
| | | | | | | | | | | | | | | },
| | | | | | | | | | | | | | },
| | | | | | | | | | | | | },
| | | | | | | | | | | | },
| | | | | | | | | | | | 
| | | | | | | | | | | | right:
| | | | | | | | | | | | {
| | | | | | | | | | | | | {
| | | | | | | | | | | | | | type: DEREF
| | | | | | | | | | | | | | exprsn:
| | | | | | | | | | | | | | {
| | | | | | | | | | | | | | | {
| | | | | | | | | | | | | | | | type: ID
| | | | | | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | | | | | varName: count
| | | | | | | | | | | | | | | },
| | | | | | | | | | | | | | },
| | | | | | | | | | | | | },
| | | | | | | | | | | | },
| | | | | | | | | | | },
| | | | | | | | | | },
| | | | | | | | | },
| | | | | | | | },
| | | | | | | | 
| | | | | | | | right:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: LIT
| | | | | | | | | | type: INT
| | | | | | | | | | val: 2
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: VAR
| | | | varName: end
| | | | varType: BYTE
| | | | isPtr: 0
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: ASSIGN
| | | | varName:
| | | | {
| | | | | {
| | | | | | type: ID
| | | | | | isPtr: 0
| | | | | | varName: end
| | | | | },
| | | | },
| | | | 
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: BINARY
| | | | | | stub: 1
| | | | | | single: 0
| | | | | | op (id): ==
| | | | | | 
| | | | | | left:
| | | | | | {
| | | | | | | {
| | | | | | | | type: ID
| | | | | | | | isPtr: 0
| | | | | | | | varName: count
| | | | | | | },
| | | | | | },
| | | | | | 
| | | | | | right:
| | | | | | {
| | | | | | | {
| | | | | | | | type: ID
| | | | | | | | isPtr: 0
| | | | | | | | varName: endAt
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: COND
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: BINARY
| | | | | | stub: 1
| | | | | | single: 0
| | | | | | op (id): !=
| | | | | | 
| | | | | | left:
| | | | | | {
| | | | | | | {
| | | | | | | | type: ID
| | | | | | | | isPtr: 112
| | | | | | | | varName: end
| | | | | | | },
| | | | | | },
| | | | | | 
| | | | | | right:
| | | | | | {
| | | | | | | {
| | | | | | | | type: LIT
| | | | | | | | type: INT
| | | | | | | | val: 0
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | | 
| | | | scope:
| | | | {
| | | | | {
| | | | | | type: ASSIGN
| | | | | | varName:
| | | | | | {
| | | | | | | {
| | | | | | | | type: DEREF
| | | | | | | | exprsn:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: count
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | },
| | | | | | 
| | | | | | exprsn:
| | | | | | {
| | | | | | | {
| | | | | | | | type: BINARY
| | | | | | | | stub: 1
| | | | | | | | single: 0
| | | | | | | | op (id): +
| | | | | | | | 
| | | | | | | | left:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: DEREF
| | | | | | | | | | exprsn:
| | | | | | | | | | {
| | | | | | | | | | | {
| | | | | | | | | | | | type: ID
| | | | | | | | | | | | isPtr: 0
| | | | | | | | | | | | varName: count
| | | | | | | | | | | },
| | | | | | | | | | },
| | | | | | | | | },
| | | | | | | | },
| | | | | | | | 
| | | | | | | | right:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: LIT
| | | | | | | | | | type: INT
| | | | | | | | | | val: 1
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | },
| | | | | },
| | | | | {
| | | | | | type: CALL
| | | | | | funcName: fizzbuzz
| | | | | | 
| | | | | | args:
| | | | | | {
| | | | | | | {
| | | | | | | | type: REF
| | | | | | | | ptr:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: count
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | | {
| | | | | | | | type: ID
| | | | | | | | isPtr: 0
| | | | | | | | varName: endAt
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: COND
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: ID
| | | | | | isPtr: 0
| | | | | | varName: end
| | | | | },
| | | | },
| | | | 
| | | | scope:
| | | | {
| | | | | {
| | | | | | type: RET
| | | | | | exprsn:
| | | | | | {
| | | | | | | {
| | | | | | | | type: LIT
| | | | | | | | type: INT
| | | | | | | | val: 0
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | },
| | },
| },
| {
| | type: FUNC
| | funcType: BYTE
| | isPtr: 0
| | isStatic: 0
| | funcName: isMultiple
| | 
| | parameters:
| | {
| | | {
| | | | type: VAR
| | | | varName: a
| | | | varType: INT
| | | | isPtr: 0
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: VAR
| | | | varName: b
| | | | varType: INT
| | | | isPtr: 0
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | },
| | 
| | scope:
| | {
| | | {
| | | | type: COND
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: BINARY
| | | | | | stub: 1
| | | | | | single: 0
| | | | | | op (id): ==
| | | | | | 
| | | | | | left:
| | | | | | {
| | | | | | | {
| | | | | | | | type: CALL
| | | | | | | | funcName: mod
| | | | | | | | 
| | | | | | | | args:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: a
| | | | | | | | | },
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: b
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | },
| | | | | | 
| | | | | | right:
| | | | | | {
| | | | | | | {
| | | | | | | | type: LIT
| | | | | | | | type: INT
| | | | | | | | val: 0
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | | 
| | | | scope:
| | | | {
| | | | | {
| | | | | | type: RET
| | | | | | exprsn:
| | | | | | {
| | | | | | | {
| | | | | | | | type: LIT
| | | | | | | | type: INT
| | | | | | | | val: 1
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: COND
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: BINARY
| | | | | | stub: 1
| | | | | | single: 0
| | | | | | op (id): !=
| | | | | | 
| | | | | | left:
| | | | | | {
| | | | | | | {
| | | | | | | | type: CALL
| | | | | | | | funcName: mod
| | | | | | | | 
| | | | | | | | args:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: a
| | | | | | | | | },
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: b
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | },
| | | | | | 
| | | | | | right:
| | | | | | {
| | | | | | | {
| | | | | | | | type: LIT
| | | | | | | | type: INT
| | | | | | | | val: 0
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | | 
| | | | scope:
| | | | {
| | | | | {
| | | | | | type: RET
| | | | | | exprsn:
| | | | | | {
| | | | | | | {
| | | | | | | | type: LIT
| | | | | | | | type: INT
| | | | | | | | val: 0
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | },
| | },
| },
| {
| | type: FUNC
| | funcType: BYTE
| | isPtr: 0
| | isStatic: 0
| | funcName: mod
| | 
| | parameters:
| | {
| | | {
| | | | type: VAR
| | | | varName: a
| | | | varType: INT
| | | | isPtr: 0
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: VAR
| | | | varName: b
| | | | varType: INT
| | | | isPtr: 0
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | },
| | 
| | scope:
| | {
| | | {
| | | | type: VAR
| | | | varName: count
| | | | varType: INT
| | | | isPtr: 0
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: ASSIGN
| | | | varName:
| | | | {
| | | | | {
| | | | | | type: ID
| | | | | | isPtr: 0
| | | | | | varName: count
| | | | | },
| | | | },
| | | | 
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 0
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: VAR
| | | | varName: out
| | | | varType: INT
| | | | isPtr: 0
| | | | isStatic: 0
| | | | isArray: 1
| | | | arrayLength:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 5
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: ASSIGN
| | | | varName:
| | | | {
| | | | | {
| | | | | | type: ID
| | | | | | isPtr: 0
| | | | | | varName: out
| | | | | },
| | | | },
| | | | 
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: LIT
| | | | | | type: INT
| | | | | | val: 0
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: CTRL
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: BINARY
| | | | | | stub: 1
| | | | | | single: 0
| | | | | | op (id): >
| | | | | | 
| | | | | | left:
| | | | | | {
| | | | | | | {
| | | | | | | | type: ID
| | | | | | | | isPtr: 0
| | | | | | | | varName: a
| | | | | | | },
| | | | | | },
| | | | | | 
| | | | | | right:
| | | | | | {
| | | | | | | {
| | | | | | | | type: ID
| | | | | | | | isPtr: 0
| | | | | | | | varName: count
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | | 
| | | | scope:
| | | | {
| | | | | {
| | | | | | type: ASSIGN
| | | | | | varName:
| | | | | | {
| | | | | | | {
| | | | | | | | type: ID
| | | | | | | | isPtr: 0
| | | | | | | | varName: count
| | | | | | | },
| | | | | | },
| | | | | | 
| | | | | | exprsn:
| | | | | | {
| | | | | | | {
| | | | | | | | type: BINARY
| | | | | | | | stub: 1
| | | | | | | | single: 0
| | | | | | | | op (id): +
| | | | | | | | 
| | | | | | | | left:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: count
| | | | | | | | | },
| | | | | | | | },
| | | | | | | | 
| | | | | | | | right:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: LIT
| | | | | | | | | | type: INT
| | | | | | | | | | val: 1
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | },
| | | | | },
| | | | | {
| | | | | | type: ASSIGN
| | | | | | varName:
| | | | | | {
| | | | | | | {
| | | | | | | | type: ID
| | | | | | | | isPtr: 0
| | | | | | | | varName: out
| | | | | | | },
| | | | | | },
| | | | | | 
| | | | | | exprsn:
| | | | | | {
| | | | | | | {
| | | | | | | | type: BINARY
| | | | | | | | stub: 1
| | | | | | | | single: 0
| | | | | | | | op (id): +
| | | | | | | | 
| | | | | | | | left:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: out
| | | | | | | | | },
| | | | | | | | },
| | | | | | | | 
| | | | | | | | right:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: LIT
| | | | | | | | | | type: INT
| | | | | | | | | | val: 1
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | },
| | | | | },
| | | | | {
| | | | | | type: COND
| | | | | | exprsn:
| | | | | | {
| | | | | | | {
| | | | | | | | type: BINARY
| | | | | | | | stub: 1
| | | | | | | | single: 0
| | | | | | | | op (id): ==
| | | | | | | | 
| | | | | | | | left:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: out
| | | | | | | | | },
| | | | | | | | },
| | | | | | | | 
| | | | | | | | right:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: b
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | },
| | | | | | 
| | | | | | scope:
| | | | | | {
| | | | | | | {
| | | | | | | | type: ASSIGN
| | | | | | | | varName:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: ID
| | | | | | | | | | isPtr: 0
| | | | | | | | | | varName: out
| | | | | | | | | },
| | | | | | | | },
| | | | | | | | 
| | | | | | | | exprsn:
| | | | | | | | {
| | | | | | | | | {
| | | | | | | | | | type: LIT
| | | | | | | | | | type: INT
| | | | | | | | | | val: 0
| | | | | | | | | },
| | | | | | | | },
| | | | | | | },
| | | | | | },
| | | | | },
| | | | },
| | | },
| | | {
| | | | type: RET
| | | | exprsn:
| | | | {
| | | | | {
| | | | | | type: ID
| | | | | | isPtr: 0
| | | | | | varName: out
| | | | | },
| | | | },
| | | },
| | },
| },
},
},
