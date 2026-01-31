# Experiment 4: Resolving Merge Conflicts

**Student:** Sakshi Pandey

## Objective
To learn how to handle merge conflicts using Git.

## Activities Completed
1. ✅ Created conflicting changes across branches
2. ✅ Simulated merge conflict scenario
3. ✅ Resolved conflict manually
4. ✅ Completed merge successfully

## Conflict Resolution Process

### Branches Created:
- **branch-a**: Production environment settings (Version 2.0, PostgreSQL, Port 8080)
- **branch-b**: Testing environment settings (Version 1.5, MongoDB, Port 5000)

### Conflict Details:
- **File**: config.txt
- **Conflicting Lines**: Version, Environment, Database, Port
- **Resolution**: Combined best features (Version 2.1, Staging environment, PostgreSQL, Port 8080)

### Commands Used:
```bash
git checkout -b branch-a
git checkout -b branch-b
git merge branch-a    # Successful merge
git merge branch-b    # Created conflict
git add config.txt    # Stage resolved file
git commit -m "..."   # Complete merge
```

### Conflict Markers:
```
<<<<<<< HEAD
(Current branch content)
=======
(Incoming branch content)
>>>>>>> branch-name
```

## Resolution Strategy
Manually edited the conflicted file to combine the best aspects of both versions, creating a staging environment configuration that maintains the newer version number and stable database choice.

**Status:** ✅ Experiment Complete