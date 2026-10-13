Добрый вечер
***
def script(check, x, y):
    return nearestgold(check, x, y)

from collections import deque

def nearestgold(check, x, y):
    if check("gold", x, y):
        return "take"

    queue = deque([(x, y, None)])
    visited = set()
    visited.add((x, y))
    directions = [(0, -1, "up"), (0, 1, "down"), (1, 0, "right"), (-1, 0, "left")]

    while queue:
        cx, cy, firststep = queue.popleft()
        for dx, dy, action in directions:
            nx, ny = cx + dx, cy + dy
            if (nx, ny) not in visited:
                curr_firststep = firststep if firststep is not None else action
                if check("gold", nx, ny):
                    return curr_firststep
                if not check("wall", nx, ny):
                    visited.add((nx, ny))
                    queue.append((nx, ny, curr_firststep))
    return "pass"
***
