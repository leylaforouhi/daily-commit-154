def rotate_strin(text, positions):
    if not text:
        return text

    positions %= len(text)
    return text[positions:] + text[:positions]


if __name__ == "__main__":
    message = "DailyCommit"
    shift = 3

    print(f"Original: {message}")
    print(f"Rotated : {rotate_string(message, shift)}")
