# Convert JSON To Typescript Interface

It is a simple electron utility project that converts JSON string to TS interface . 
When front end developers need to contruct Type Script Interfaces from sample api input ouput JSON, this may save their time.

## Usage

### Build Binary Executable

```bash
 git clone https://github.com/debonil/generate-ts-interface.git
 cd generate-ts-interface/
 npm i
 npm run make
```
 Platform specific  Binary Executable will be ready.
Now run the application

### Example

Input: 
``` typescript

{
  "name":"John",
  "age":30,
  "cars": {
    "car1":"Ford",
    "car2":"BMW",
    "car3":"Fiat"
  }
 }

```

Output :
``` typescript

export  interface  INTERFACE_NAME  {
	name:    string; // John
	age:    number; // 30
	cars:    {
		car1:    string; // Ford
		car2:    string; // BMW
		car3:    string; // Fiat
		}; // [object Object]
	}

```

Enjoy your time!!!

