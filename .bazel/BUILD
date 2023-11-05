load("@rules_php//php:rules.bzl", "php_binary", "php_test")

# Aturan untuk mengkompilasi PHP binary
php_binary(
    name = "laravel_app",
    srcs = glob(["app/**/*.php", "bootstrap/**/*.php", "public/**/*.php"]),
    entry_script = "public/index.php",
)

# Aturan untuk menjalankan pengujian PHP
php_test(
    name = "laravel_tests",
    srcs = glob(["tests/**/*.php"]),
    entry_script = "tests/run-tests.php",
)