# Hashing Passwords

This script allows you to hash passwords using various hash algorithms. By hashing passwords, you can securely store and compare them without revealing the original passwords.

## Execution

To run the script, use the following command:

```shell
python hashing_passwords.py <password> [-t {sha256,sha512,md5}]
```

- `<password>`: The password you want to hash.
- `-t {sha256, sha512, md5}` (optional): The hash algorithm to use. The default hash algorithm is `sha256`.

## Example

```shell
$ python hashing_passwords.py nakao
< hash-type: sha256 >
63201414e0804bdc63b662bd87f0f51616ab69bd672aefe2b17fcec1ef14a995
```

```shell
$ python hashing_passwords.py nakao -t sha512
< hash-type: sha512 >
9cae3a2096c33b6049502ac923baff9649478df62eb090bac30d5c684b2f724ecaf7c3d7744ebccb49118d2ab07d615b02a7d170fd6310f815da18e09863841a
```

## Supported Hash Algorithms

The script supports the following hash algorithms:

- `sha256` (default)
- `sha512`
- `md5`

## Note

Hashing passwords provides a one-way transformation, making it difficult to reverse-engineer the original password. However, please note that using a strong and unique password is still crucial for security. Additionally, it's recommended to use more secure hash algorithms like `sha512` instead of `md5`.

## Contribution

Contributions are welcome! If you have any suggestions or improvements, please create a pull request or open an issue.

## License

This project is licensed under the [MIT License](LICENSE).