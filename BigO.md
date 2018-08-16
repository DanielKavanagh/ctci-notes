## Big O

Defines the efficiency of a program, in both time and space.

In acedemia there's three different concepts:

`Big O` - Describes the upper bound on time. An algorithm that prints all the values of an array could be described as O(N), but also O(N²) or O(N³) or O(N¹⁰⁰) in an academic setting.

`Big Ω (Big Omega)` - Describes the lower bound on time. Similarly, printing the values of an array could be Ω(N) or Ω(log N) or Ω(1).

`Big Θ (Big Theta)` - Means both Big Ω and Big O. Gives a tight bound on runtime. 

In development, Big O is basically Big Θ. 

## Comments

- Big O describes the rate of increase on time, its possible for O(N) to be faster than O(1) with a particular set of inputs.

- When calculating Big O, constants should be dropped. Describing an algorithm as O(2N) can be simplified to O(N)

![BigOGraph](https://he-s3.s3.amazonaws.com/media/uploads/ece920b.png)

```
for (int a : arrA) {
	print(a);
}

for (int b : arrB) {
	print(b);
}
```

- Add the runtimes (do this then do that), O(A + B)

```
for (int a : arrA) {
	for (int b : arrB) {
		print(a + "," + b);
	}
}
```

- Multiply the runtimes (for every time you do this, do that), O(A * B)