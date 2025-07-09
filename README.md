# 🧩 Trexquant Hangman Problem - Global Alpha Researcher

## 🧠 Approach Summary

This solution uses a regex-based filtering strategy combined with n-gram and bigram frequency models.  
It ranks unguessed letters by their likelihood across matching word candidates, with a vowel density heuristic to avoid early vowel guessing.  
Fallback heuristics use substring matching (0.75, 0.5, 0.33 of word length) to recover from difficult matches.  
When no strong match is found, it defaults to global letter frequency across the training corpus.  

## 📁 Project Structure

```
├── finalt1.ipynb              # Main notebook containing the full implementation and logic
├── words_250000_train.txt     # Full dictionary used for filtering and frequency analysis
├── Anshuman_Hangman_Report.pdf  # Summary report of the approach and findings
├── README.md                  # This readme file
├── LICENSE                    # Open source license (MIT)

## 📊 Performance Observations

- ✅ ~64% win rate for first 40 practice games  
- ✅ ~60%+ win rate across 150 practice games  
- 📉 Final win rate dropped to **57.5%** after completing 1000 recorded games
