# genpasswd

`genpasswd` is a simple and lightweight Bash script to generate random passwords of customizable length and complexity.

## Features

- Generate passwords with customizable **length** and **complexity level**
- Supports **3 levels of password strength**:
    - **Level 1**: Alphabhetic Characters only(A-Z, a-z)
    - **Level 2**: AlphaNumeric Characters (A-Z, a-z, 0-9)
    - **Level 3**: AlphaNumeric with Special Characters (A-Z, a-z, 0-9,  @#$%&?><)


## Usage

```bash
./genpasswd.sh -l <length> -L <level>

```

You can provide the arguments in any of the following combinations:

- Option 1: Specify either length or level

```bash
./genpasswd.sh -l 12   # Generate 12-character password with default level 1
./genpasswd.sh -L 3    # Generate default length password (8-characters) with level 3
```

- Option 2: Specify both

```bash
./genpasswd.sh -l 16 -L 2    # Generates 16-character alphanumeric password
./genpasswd.sh -L 2 -l 10    # Generates 10-character alphanumeric password
```

## Examples

```bash
$ ./genpasswd.sh -l 12 -L 1
eMKkvHWyMFyv

$ ./genpasswd.sh -l 10 -L 2
lRDWoWjk1S    

$ ./genpasswd.sh -l 14 -L 3
pC$A?b&#3#9@>y
```

## Contribution

You are free to contribute to make this utility more efficient and useful.

***Happy Password Generating!***
