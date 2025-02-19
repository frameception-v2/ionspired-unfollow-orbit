### Step 1: Initialize Basic Frame Structure
```text
1. Create foundational HTML template for frame UI
2. Setup server endpoint to handle POST requests
3. Implement basic refresh button functionality
```

### Step 2: Implement State Payload Management
```text
1. Add payload decoding/encoding utilities
2. Create state schema for previous followers and unfollows
3. Integrate state handling in POST route (Reference Step 1)
```

### Step 3: Integrate Follower API Client
```text
1. Create API client for Farcaster followers endpoint
2. Implement pagination handling for >500 followers
3. Add response caching with TTL (Reference Step 2)
```

### Step 4: Develop Unfollow Detection Logic
```text
1. Implement set comparison between current/previous followers
2. Generate unfollow events with timestamps
3. Merge new unfollows with existing state (Reference Step 2-3)
```

### Step 5: Build Dynamic Unfollow Display
```text
1. Create template helpers for rendering user profiles
2. Implement time-sorted grid layout from spec
3. Add empty state handling (Reference Step 1 & 4)
```

### Step 6: Add Error Handling System
```text
1. Implement API retry logic with exponential backoff
2. Create error state templates
3. Add payload corruption recovery (Reference Step 2 & 3)
```

### Step 7: Optimize Payload Compression
```text
1. Implement FID list compression algorithm
2. Convert timestamps to UNIX format
3. Validate payload size limits (Reference Step 1 & 2)
```

### Step 8: Finalize Refresh Functionality
```text
1. Implement state-preserving refresh action
2. Add loading indicators during API calls
3. Validate real-time detection (Reference Step 4 & 5)
```

### Step 9: Edge Case Handling
```text
1. Add duplicate unfollow prevention
2. Implement user reactivation detection
3. Add input validation for FIDs (Reference Step 4 & 6)
```

### Step 10: Final Integration Testing
```text
1. Validate full user flow with state persistence
2. Test payload size boundaries
3. Verify error scenarios (Reference all previous steps)
```