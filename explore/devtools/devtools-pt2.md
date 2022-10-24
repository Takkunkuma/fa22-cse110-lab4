1. The bug was that the arithmatic sum was being performed in string, so it simply concatenated two user inputs.
2. My fix was to wrap each number input by parseInt function.