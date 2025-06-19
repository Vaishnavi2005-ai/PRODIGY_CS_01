def caesar_cipher_encrypt(text, shift):
    result = ""
    for char in text:
        if char.isalpha():
            start = ord('A') if char.isupper() else ord('a')
            result += chr((ord(char) - start + shift) % 26 + start)
        else:
            result += char
    return result

def caesar_cipher_decrypt(text, shift):
    return caesar_cipher_encrypt(text, -shift)

# Main function
def main():
    print("Caesar Cipher Program")
    choice = input("Type 'e' to encrypt or 'd' to decrypt: ").lower()
    message = input("Enter the message: ")
    shift = int(input("Enter the shift value: "))

    if choice == 'e':
        encrypted = caesar_cipher_encrypt(message, shift)
        print("Encrypted message:", encrypted)
    elif choice == 'd':
        decrypted = caesar_cipher_decrypt(message, shift)
        print("Decrypted message:", decrypted)
    else:
        print("Invalid choice! Please type 'e' or 'd'.")

if __name__ == "__main__":
    main()
