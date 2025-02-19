```markdown
### Core
1. [ ] Create foundational HTML template for frame UI  
   **Validation:** Basic frame structure visible in browser
2. [ ] Setup server endpoint to handle POST requests  
   **Validation:** POST requests received at `/api/frame`
3. [ ] Add payload decoding/encoding utilities  
   **Validation:** Round-trip encode/decode test passes
4. [ ] Create state schema for previous followers/unfollows  
   **Validation:** Schema validates sample follower data
5. [ ] Integrate state handling in POST route  
   **Validation:** State persists between requests
6. [ ] Implement response caching with TTL  
   **Validation:** Subsequent API calls hit cache
7. [ ] Implement set comparison between current/previous followers  
   **Validation:** Detects added/removed FIDs
8. [ ] Generate unfollow events with timestamps  
   **Validation:** Events contain valid UNIX timestamps
9. [ ] Merge new unfollows with existing state  
   **Validation:** State shows cumulative unfollow history
10. [ ] Implement FID list compression algorithm  
    **Validation:** 50%+ reduction in payload size
11. [ ] Convert timestamps to UNIX format  
    **Validation:** All timestamps in numeric format
12. [ ] Add duplicate unfollow prevention  
    **Validation:** Duplicate FIDs filtered
13. [ ] Implement user reactivation detection  
    **Validation:** Re-follows clear unfollow status

### API
1. [ ] Create API client for Farcaster followers endpoint  
    **Validation:** Returns follower list for test FID
2. [ ] Implement pagination handling for >500 followers  
    **Validation:** Returns complete follower set
3. [ ] Implement API retry logic with exponential backoff  
    **Validation:** Recovers from 3 consecutive failures

### UI
1. [ ] Implement basic refresh button functionality  
    **Validation:** Click triggers frame reload
2. [ ] Create template helpers for rendering user profiles  
    **Validation:** Displays username + PFP mockup
3. [ ] Implement time-sorted grid layout from spec  
    **Validation:** Items ordered newest-first
4. [ ] Add empty state handling  
    **Validation:** Shows "No unfollows" message
5. [ ] Create error state templates  
    **Validation:** Displays error message + retry button
6. [ ] Add loading indicators during API calls  
    **Validation:** Spinner appears during requests
```