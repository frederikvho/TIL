ERROR 1273 (HY000) at line 1: Unknown collation: 'utf8mb4_0900_ai_ci'
Import failed.
sed -i '' 's/utf8mb4_0900_ai_ci/utf8mb4_unicode_ci/g' source.sql
