# What is a hash function?

- **one-way function** - it's easy to compute the hash, but hard to find the input
- **deterministic** - the same input always produces the same output
- **collision-resistant** - it's hard to find two different inputs that produce the same output
- **accept any input size** - 
- **output should have bounded size** - 
- **be fast to compute**

## Usage

- **representation of data object** - history, state, etc
- **keys in db** - to encrypt a message
- **digital signatures** - to prove that the message was sent by the right person
- **key derivation** - to generate a key from a password
- **pseudo-random numbers** - to generate a random number