# Acceptance Criteria (Given/When/Then)

## AC1 Begin (`b`)
Given the app is open  
When user presses `b`  
Then a new active polyline is created (until max 100)

## AC2 Move (`m`)
Given there is at least 1 polyline with points  
When user presses `m` and drags near a point  
Then the closest point moves with the mouse

## AC3 Delete (`d`)
Given there is at least 1 polyline with points  
When user presses `d` and clicks near a point  
Then the point is removed and the polyline updates

## AC4 Refresh (`r`)
Given there are polylines in memory  
When user presses `r`  
Then canvas is cleared and all polylines are redrawn

## AC5 Quit (`q`)
Given the app is running  
When user presses `q`  
Then the session exits (web: either clears state or disables further input and displays an exit message)
