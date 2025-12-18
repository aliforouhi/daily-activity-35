# daily_update.p
import datetime
import random

print("Daily GitHub activity - Day 35")

today = datetime.date.today()

# Generate random scores and classify them
scores = [random.randint(0, 100) for _ in range(8)]

passed = [s for s in scores if s >= 50]
failed = [s for s in scores if s < 50]

print(f"Today's date: {today}")
print("Scores:", scores)
print("Passed scores:", passed)
print("Failed scores:", failed)
print("Pass rate:", f"{len(passed)}/{len(scores)}")
