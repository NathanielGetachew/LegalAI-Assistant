# Pseudocode logic inside notebook:
for _ in range(N):  # e.g., N = 5
    result = model.generate_content(prompt)
    responses.append(result.text)

# Then apply:
- Majority voting or heuristic analysis
- Select the most frequent or plausible classification
