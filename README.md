# 🧩 Trexquant Hangman Problem - Global Alpha Researcher

## 🧠 Approach Summary

This solution uses a regex-based filtering strategy combined with n-gram and bigram frequency models.  
It ranks unguessed letters by their likelihood across matching word candidates, with a vowel density heuristic to avoid early vowel guessing.  
Fallback heuristics use substring matching (0.75, 0.5, 0.33 of word length) to recover from difficult matches.  
When no strong match is found, it defaults to global letter frequency across the training corpus.  

## 📊 Performance Observations

- ✅ ~64% win rate for first 40 practice games  
- ✅ ~60%+ win rate across 150 practice games  
- 📉 Final win rate dropped to **57.5%** after completing 1000 recorded games
