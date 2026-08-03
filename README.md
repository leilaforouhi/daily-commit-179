def separate_by_length(words, limit):
    short_words = []
    long_words = []

    for word in words:
        if len(word) <= limit:
            short_words.append(word)
        else:
            long_words.append(word)

    return short_words, long_words


if __name__ == "__main__":
    words = [
        "code",
        "python",
        "development",
        "git",
        "repository"
    ]

    short, long = separate_by_length(words, 5)

    print(f"Short words: {short}")
    print(f"Long words: {long}")
