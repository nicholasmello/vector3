#Go Vector 3 Library

This repository holds a library containing 3 dimensional vectors for Go. It was created to help with calculations for my Rocket League bot. Package uses float32 because that is what RLBot uses.

##Instillation
From the command line run the command 
`go get github.com/xonmello/vector3`
Then import it at the top of your go project
`import "github.com/xonmello/vector3"`

##Usage
Vectors can be created with the New function and calculations can be done with the functions below
* Dot - Dot Product Between 2 Vectors
* Cross - Cross Product Between 2 Vectors
* Add - Adds Vectors together
* AddScalar - Adds a scalar to all terms of a Vector
* Subtract - Subtracts Vectors
* SubtractScalar - Subtracts a scalar from all terms of a Vector
* Divide - Divides Vectors
* DivideScalar - Divides a scalar from all terms of a Vector
* Magnitude - Returns the magnitude of the vector
* Distance - Returns the distance between 2 vectors

##Examples
```golang
a := Vector3.New(1,2,3)
b := Vector3.New(-3,2,3)
fmt.Println(a.Add(b))
```
```golang
a := Vector3.New(1,2,3)
b := Vector3.New(-3,2,3)
fmt.Println(a.Distance(b))
```
```golang
a := Vector3.New(1,2,3)
fmt.Println(a.AddScalar(5))
```
```golang
a := Vector3.New(1,2,3)
b := Vector3.New(-7,6,12)
fmt.Println(a.Cross(b))
```