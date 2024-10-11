# posipercentgrade

lame % = ( number / number ) * 100 converter that i originally wrote in swift but asked claude to re-write it in html with a basic gui that i slightly customized.

**initial swift code:**

```swift
let totalExamScore: Double = 100
var highestScore: Double? = nil
var myScore: Double? = nil

func didPass(highestScore: Double, myScore: Double) -> String {
    let newPassingScore = highestScore * 0.75
    let printPercent = (myScore / highestScore) * 100
    
    
    if myScore >= newPassingScore {
        return "Passed! You got \(printPercent)%."
    } else {
        return "Failed! You got \(printPercent)%."
    }
}

print(didPass(highestScore: 92, myScore: 86))
```
