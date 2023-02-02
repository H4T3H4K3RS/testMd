

# **Solution**

```bash
#!/bin/bash
a=10
c=10
b=20

while [[ $a -lt $b ]]
do
	c=$((c-a))
	func $a $c
	a=$((a+1))
	f=$((a%2))
	if [[ $f == 0 ]]; then
		echo "Current value of variable a is $a"
	fi
done

func(){
	local a=$1
	local b=$2
	echo "Function took two numbers: $a and $b"
}
```