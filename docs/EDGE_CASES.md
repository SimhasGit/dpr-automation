# Edge Cases to Handle

## Priority 1 — Input Validation
- [ ] Employee sends empty message
- [ ] Employee sends only image/voice note (no text)
- [ ] Employee sends in different language (Kannada, Hindi)
- [ ] Employee sends very long message (Gemini token limit)
- [ ] Employee sends gibberish or irrelevant text
- [ ] Employee messages outside working hours

## Priority 2 — Identity Issues
- [ ] Two employees with same first name
- [ ] Employee doesn't mention name in message
- [ ] New employee who hasn't registered yet
- [ ] Employee uses someone else's Telegram

## Priority 3 — System Failures
- [ ] Gemini API is down
- [ ] Gmail quota exceeded (500/day limit)
- [ ] Supabase is sleeping (free tier spins down)
- [ ] ngrok URL changed and webhook is broken
- [ ] n8n crashes mid-workflow
- [ ] Employee sends duplicate report same day

## Priority 4 — Data Integrity
- [ ] Gemini formats report but misses a section
- [ ] Report saved to Supabase but email fails
- [ ] Email sent but Supabase save fails
- [ ] Special characters in message break JSON

## Notes
- Solve in priority order
- Each fix should be tested end-to-end before moving to next
- Document the fix below each item once resolved
