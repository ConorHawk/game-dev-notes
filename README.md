# Handy unity info

###Physics Movement

```C#
void FixedUpdate () {
	rb.AddForce(0,0,forwardForce * Time.deltaTime);
}
```

```C#
FindObjectOfType<GameManager>().EndGame();
```