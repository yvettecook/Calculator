## CalculatorApp

Basic calculator app, and the first assignment of the Stanford University `Developing iOS 8 Apps with Swift` course.

### Key Learnings:

- [x] Closures

`performOperation( { (op1, op2) in return op1 * op2 })`

- [x] Refactoring Closures!

`performOperation( { $0 * $1 } )`

- [x] Enums

``` enum Op {
        case Operand(Double)
        case UnaryOperation(String, Double -> Double)
        case BinaryOperation(String, (Double, Double) -> Double)```

- [x] Computed Properties

``` var description : String {
            get {
                switch self {
                case .Operand(let value):
                    return "\(value)"
                case .UnaryOperation(let string, _):
                    return string
                case .BinaryOperation(let string, _):
                    return string
                }
            }
    }```

- [x] Recursion
