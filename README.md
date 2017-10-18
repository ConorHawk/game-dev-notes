# Handy unity info

###Physics Movement
 test 
```C#
void FixedUpdate () {
	rb.AddForce(0,0,forwardForce * Time.deltaTime);
}
```

```C#
FindObjectOfType<GameManager>().EndGame();
```