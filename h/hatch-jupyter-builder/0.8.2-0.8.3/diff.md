# Comparing `tmp/hatch_jupyter_builder-0.8.2.tar.gz` & `tmp/hatch_jupyter_builder-0.8.3.tar.gz`

## Comparing `hatch_jupyter_builder-0.8.2.tar` & `hatch_jupyter_builder-0.8.3.tar`

### file list

```diff
@@ -1,128 +1,130 @@
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/.readthedocs.yml
--rw-r--r--   0        0        0    22893 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/CHANGELOG.md
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/RELEASE.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/codecov.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/docs/Makefile
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/docs/conf.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/docs/make.bat
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/docs/source/background/index.rst
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/docs/source/get_started/config.md
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/docs/source/get_started/index.rst
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/docs/source/how_to_guides/index.rst
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/docs/source/how_to_guides/migrating_data_files_projects.md
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/docs/source/how_to_guides/migrating_javascript_projects.md
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/docs/source/reference/api_docs.rst
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/docs/source/reference/index.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/__main__.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/cli.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/hooks.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/plugin.py
--rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/compare_migrated/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/compare_migrated/__main__.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/compare_migrated/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/migrate/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/migrate/__main__.py
--rw-r--r--   0        0        0     8131 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/migrate/_migrate.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/migrate/cli.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/migrate/jupyter_packaging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/__init__.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/conftest.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/test_hooks.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/test_is_stale.py
--rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/test_migration.py
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/test_npm_builder.py
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/test_plugin.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/test_utils.py
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/pyproject.toml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/.eslintignore
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/.eslintrc.js
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/.gitignore
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/.npmignore
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/.prettierignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/.prettierrc
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/LICENSE.txt
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/MANIFEST.in
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/README.md
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/babel.config.js
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/codecov.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/install.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/jest.config.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject.json
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/package.json
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/pyproject.toml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/readthedocs.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/setup.cfg
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/setup.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/tsconfig.eslint.json
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/tsconfig.json
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/webpack.config.js
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/.github/workflows/build.yml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/css/widget.css
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/Makefile
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/environment.yml
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/make.bat
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/source/conf.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/source/develop-install.rst
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/source/index.rst
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/source/installing.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/source/introduction.rst
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/source/_static/helper.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/source/examples/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/source/examples/introduction.nblink
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/examples/introduction.ipynb
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject/__init__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject/_frontend.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject/_version.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject/example.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject/nbextension/extension.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject/tests/__init__.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject/tests/conftest.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject/tests/test_example.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/extension.ts
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/index.ts
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/plugin.ts
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/version.ts
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/widget.ts
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/__tests__/utils.ts
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/pyproject.toml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/.eslintignore
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/.eslintrc.js
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/.gitignore
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/CHANGELOG.md
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/LICENSE
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/MANIFEST.in
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/README.md
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/RELEASE.md
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/install.json
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/package.json
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/pyproject.toml
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/tsconfig.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/.github/workflows/build.yml
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/.github/workflows/check-release.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/myextension/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/myextension/_version.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/schema/plugin.json
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/style/index.css
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/style/index.js
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/LICENSE.txt
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/README.md
--rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/.readthedocs.yml
+-rw-r--r--   0        0        0    24723 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/CHANGELOG.md
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/RELEASE.md
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/Makefile
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/conf.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/make.bat
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/source/background/index.rst
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/source/get_started/config.md
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/source/get_started/index.rst
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/source/how_to_guides/index.rst
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/source/how_to_guides/migrating_data_files_projects.md
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/source/how_to_guides/migrating_javascript_projects.md
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/source/reference/index.rst
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/source/reference/api/hatch_jupyter_builder.compare_migrated.rst
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/source/reference/api/hatch_jupyter_builder.migrate.rst
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/source/reference/api/hatch_jupyter_builder.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/docs/source/reference/api/modules.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/__main__.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/cli.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/hooks.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/plugin.py
+-rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/compare_migrated/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/compare_migrated/__main__.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/compare_migrated/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/migrate/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/migrate/__main__.py
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/migrate/_migrate.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/migrate/cli.py
+-rw-r--r--   0        0        0     5130 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/migrate/jupyter_packaging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/__init__.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/conftest.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/test_hooks.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/test_is_stale.py
+-rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/test_migration.py
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/test_npm_builder.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/test_plugin.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/test_utils.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/pyproject.toml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/.eslintignore
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/.eslintrc.js
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/.gitignore
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/.npmignore
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/.prettierignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/.prettierrc
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/LICENSE.txt
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/MANIFEST.in
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/README.md
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/babel.config.js
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/codecov.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/install.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/jest.config.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject.json
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/package.json
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/pyproject.toml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/readthedocs.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/setup.cfg
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/setup.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/tsconfig.eslint.json
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/tsconfig.json
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/webpack.config.js
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/.github/workflows/build.yml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/css/widget.css
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/Makefile
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/environment.yml
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/make.bat
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/source/conf.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/source/develop-install.rst
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/source/index.rst
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/source/installing.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/source/introduction.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/source/_static/helper.js
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/source/examples/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/source/examples/introduction.nblink
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/examples/introduction.ipynb
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject/__init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject/_frontend.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject/_version.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject/example.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject/nbextension/extension.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject/tests/__init__.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject/tests/conftest.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject/tests/test_example.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/extension.ts
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/index.ts
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/plugin.ts
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/version.ts
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/widget.ts
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/__tests__/utils.ts
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/pyproject.toml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/.eslintignore
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/.eslintrc.js
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/.gitignore
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/CHANGELOG.md
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/LICENSE
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/MANIFEST.in
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/README.md
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/RELEASE.md
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/install.json
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/package.json
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/pyproject.toml
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/tsconfig.json
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/myextension/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/myextension/_version.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/schema/plugin.json
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/style/index.css
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/style/index.js
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/LICENSE.txt
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/README.md
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 hatch_jupyter_builder-0.8.3/PKG-INFO
```

### Comparing `hatch_jupyter_builder-0.8.2/.pre-commit-config.yaml` & `hatch_jupyter_builder-0.8.3/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 ci:
   autoupdate_schedule: monthly
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
-      - id: end-of-file-fixer
       - id: check-case-conflict
+      - id: check-ast
+      - id: check-docstring-first
       - id: check-executables-have-shebangs
-      - id: requirements-txt-fixer
       - id: check-added-large-files
       - id: check-case-conflict
+      - id: check-merge-conflict
+      - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
-      - id: forbid-new-submodules
-      - id: check-builtin-literals
+      - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.19.2
+    rev: 0.22.0
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
 
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.177
+    rev: v0.0.260
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `hatch_jupyter_builder-0.8.2/CHANGELOG.md` & `hatch_jupyter_builder-0.8.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,35 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.8.3
+
+([Full Changelog](https://github.com/jupyterlab/hatch-jupyter-builder/compare/v0.8.2...110ef7d5cc4b6118d21c130965f6e88ddf31ff22))
+
+### Maintenance and upkeep improvements
+
+- Use local coverage [#114](https://github.com/jupyterlab/hatch-jupyter-builder/pull/114) ([@blink1073](https://github.com/blink1073))
+- Add more linting [#106](https://github.com/jupyterlab/hatch-jupyter-builder/pull/106) ([@blink1073](https://github.com/blink1073))
+- Fix test typing [#104](https://github.com/jupyterlab/hatch-jupyter-builder/pull/104) ([@blink1073](https://github.com/blink1073))
+- Add more ci checks [#102](https://github.com/jupyterlab/hatch-jupyter-builder/pull/102) ([@blink1073](https://github.com/blink1073))
+
+### Documentation improvements
+
+- Add license classifier [#111](https://github.com/jupyterlab/hatch-jupyter-builder/pull/111) ([@fcollonval](https://github.com/fcollonval))
+- Add full api docs [#103](https://github.com/jupyterlab/hatch-jupyter-builder/pull/103) ([@blink1073](https://github.com/blink1073))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab/hatch-jupyter-builder/graphs/contributors?from=2022-12-13&to=2023-04-14&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyterlab%2Fhatch-jupyter-builder+involves%3Ablink1073+updated%3A2022-12-13..2023-04-14&type=Issues) | [@codecov](https://github.com/search?q=repo%3Ajupyterlab%2Fhatch-jupyter-builder+involves%3Acodecov+updated%3A2022-12-13..2023-04-14&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyterlab%2Fhatch-jupyter-builder+involves%3Afcollonval+updated%3A2022-12-13..2023-04-14&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyterlab%2Fhatch-jupyter-builder+involves%3Apre-commit-ci+updated%3A2022-12-13..2023-04-14&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.8.2
 
 ([Full Changelog](https://github.com/jupyterlab/hatch-jupyter-builder/compare/v0.8.1...dacbd9ba0115b0991870bf2b7d741ada0d1d4ffd))
 
 ### Enhancements made
 
 - Adopt ruff and reduce pre-commit usage [#97](https://github.com/jupyterlab/hatch-jupyter-builder/pull/97) ([@blink1073](https://github.com/blink1073))
@@ -27,16 +51,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab/hatch-jupyter-builder/graphs/contributors?from=2022-10-14&to=2022-12-13&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Ajupyterlab%2Fhatch-jupyter-builder+involves%3Ablink1073+updated%3A2022-10-14..2022-12-13&type=Issues) | [@codecov](https://github.com/search?q=repo%3Ajupyterlab%2Fhatch-jupyter-builder+involves%3Acodecov+updated%3A2022-10-14..2022-12-13&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyterlab%2Fhatch-jupyter-builder+involves%3Apre-commit-ci+updated%3A2022-10-14..2022-12-13&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.8.1
 
 ([Full Changelog](https://github.com/jupyterlab/hatch-jupyter-builder/compare/v0.8.0...8257c8561d946def6193ad63afa446e0b261cb39))
 
 ### Bugs fixed
 
 - Fix handling of bool args [#82](https://github.com/jupyterlab/hatch-jupyter-builder/pull/82) ([@blink1073](https://github.com/blink1073))
```

### Comparing `hatch_jupyter_builder-0.8.2/RELEASE.md` & `hatch_jupyter_builder-0.8.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/.github/workflows/prep-release.yml` & `hatch_jupyter_builder-0.8.3/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/.github/workflows/publish-release.yml` & `hatch_jupyter_builder-0.8.3/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/.github/workflows/tests.yml` & `hatch_jupyter_builder-0.8.3/.github/workflows/tests.yml`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,18 @@
     branches: [main]
   pull_request:
   schedule:
     # Run weekly
     # * is a special character in YAML so you have to quote this string
     - cron: "0 0 * * 0"
 
+defaults:
+  run:
+    shell: bash -eux {0}
+
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
@@ -32,18 +36,23 @@
         run: hatch run cov:test
       - name: Run cli checks
         run: |
           pip install -e .
           hatch-jupyter-builder -h
           hatch-jupyter-builder migrate -h
           hatch-jupyter-builder compare-migrated -h
-      - name: Code coverage
-        run: |
-          pip install codecov coverage[html]
-          codecov
+      - uses: jupyterlab/maintainer-tools/.github/actions/upload-coverage@v1
+
+  coverage:
+    runs-on: ubuntu-latest
+    needs:
+      - build
+    steps:
+      - uses: actions/checkout@v3
+      - uses: jupyterlab/maintainer-tools/.github/actions/report-coverage@v1
 
   check_release:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - uses: jupyter-server/jupyter_releaser/.github/actions/check-release@v2
@@ -64,31 +73,40 @@
     steps:
       - uses: actions/checkout@v2
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - name: Run Migration Tests
         run: hatch run migration:test
 
   test_docs:
-    runs-on: ubuntu-latest
+    runs-on: windows-latest
     steps:
       - uses: actions/checkout@v2
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
+      - name: Build API docs
+        run: |
+          hatch run docs:api
+          # If this fails run `hatch run docs:api` locally
+          # and commit.
+          git status --porcelain
+          git status -s | grep "A" && exit 1
+          git status -s | grep "M" && exit 1
+          echo "API docs done"
       - run: hatch run docs:build
 
   test_lint:
     name: Test Lint
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       -  name: Run Linters
          run: |
           hatch run typing:test
           hatch run lint:style
-          pipx run 'validate-pyproject[all]' pyproject.toml
+          pipx run interrogate -v .
           pipx run doc8 --max-line-length=200  --ignore-path=docs/source/other/full-config.rst
 
   test_minimum_versions:
     name: Test Minimum Versions
     timeout-minutes: 20
     runs-on: ubuntu-latest
     steps:
@@ -131,15 +149,15 @@
       - uses: jupyterlab/maintainer-tools/.github/actions/test-sdist@v1
         with:
           test_command: hatch run test:test
 
   tests_check: # This job does nothing and is only used for the branch protection
     if: always()
     needs:
-      - build
+      - coverage
       - migration
       - test_lint
       - test_docs
       - test_minimum_versions
       - test_prereleases
       - check_links
       - check_release
```

### Comparing `hatch_jupyter_builder-0.8.2/docs/Makefile` & `hatch_jupyter_builder-0.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/docs/conf.py` & `hatch_jupyter_builder-0.8.3/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,27 @@
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ["sphinx.ext.napoleon", "sphinx.ext.autodoc", "myst_parser"]
+extensions = [
+    "sphinx.ext.napoleon",
+    "sphinx.ext.autodoc",
+    "myst_parser",
+    "sphinx_autodoc_typehints",
+]
+
+try:
+    import enchant  # type:ignore  # noqa
+
+    extensions += ["sphinxcontrib.spelling"]
+except ImportError:
+    pass
 
 myst_enable_extensions = ["html_image"]
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
@@ -49,14 +61,17 @@
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "pydata_sphinx_theme"
 
+# Example configuration for intersphinx: refer to the Python standard library.
+intersphinx_mapping = {"python": {"https://docs.python.org/3/": None}}
+
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # html_static_path = ["_static"]
 
 
 import os.path as osp
```

### Comparing `hatch_jupyter_builder-0.8.2/docs/index.rst` & `hatch_jupyter_builder-0.8.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/docs/make.bat` & `hatch_jupyter_builder-0.8.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/docs/source/background/index.rst` & `hatch_jupyter_builder-0.8.3/docs/source/background/index.rst`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/docs/source/get_started/config.md` & `hatch_jupyter_builder-0.8.3/docs/source/get_started/config.md`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/docs/source/how_to_guides/migrating_data_files_projects.md` & `hatch_jupyter_builder-0.8.3/docs/source/how_to_guides/migrating_data_files_projects.md`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/docs/source/how_to_guides/migrating_javascript_projects.md` & `hatch_jupyter_builder-0.8.3/docs/source/how_to_guides/migrating_javascript_projects.md`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/cli.py` & `hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+"""The cli implementation for hatch_jupyter_builder."""
 import argparse
 import sys
 from typing import Optional
 
 from .compare_migrated import cli as compare_cli
 from .migrate import cli as migrate_cli
 
 
 def make_parser(
     parser: Optional[argparse.ArgumentParser] = None, prog: Optional[str] = None
 ) -> argparse.ArgumentParser:
+    """Make an arg parser."""
     if parser is None:
         parser = argparse.ArgumentParser(prog=prog)
     parsers = parser.add_subparsers()
 
     migrate_parser = parsers.add_parser("migrate")
     migrate_cli.make_parser(migrate_parser)
     migrate_parser.set_defaults(func=migrate_cli.run)
@@ -21,14 +23,15 @@
     compare_cli.make_parser(compare_parser)
     compare_parser.set_defaults(func=compare_cli.run)
 
     return parser
 
 
 def run(args: Optional[argparse.Namespace] = None) -> None:
+    """Run the main script."""
     if args is None:
         prog = (
             f"{sys.executable} -m hatch_jupyter_builder"
             if sys.argv[0].endswith("__main__.py")
             else None
         )
         parser = make_parser(prog=prog)
```

### Comparing `hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/plugin.py` & `hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""The main plugin for hatch_jupyter_builder."""
 import os
 import typing as t
 import warnings
 from dataclasses import dataclass, field, fields
 
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 
@@ -25,17 +26,20 @@
     editable_build_kwargs: t.Mapping[str, str] = field(default_factory=dict)
     ensured_targets: t.List[str] = field(default_factory=list)
     skip_if_exists: t.List[str] = field(default_factory=list)
     optional_editable_build: str = ""
 
 
 class JupyterBuildHook(BuildHookInterface):
+    """The hatch jupyter builder build hook."""
+
     PLUGIN_NAME = "jupyter-builder"
 
     def initialize(self, version, build_data):
+        """Initialize the plugin."""
         log = _get_log()
         log.info("Running jupyter-builder")
         if self.target_name not in ["wheel", "sdist"]:
             log.info(f"ignoring target name {self.target_name}")
             return False
 
         if os.getenv("SKIP_JUPYTER_BUILDER"):
@@ -74,15 +78,15 @@
             build_kwargs = normalize_kwargs(build_kwargs)
             log.info(f"Building with {config.build_function}")
             log.info(f"With kwargs: {build_kwargs}")
             try:
                 build_func(self.target_name, version, **build_kwargs)
             except Exception as e:
                 if version == "editable" and config.optional_editable_build.lower() == "true":
-                    warnings.warn(f"Encountered build error:\n{e}")
+                    warnings.warn(f"Encountered build error:\n{e}")  # noqa B028
                 else:
                     raise e
         else:
             log.info("Skipping build")
 
         # Ensure targets in distributable dists.
         if version == "standard":
```

### Comparing `hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/utils.py` & `hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Utilities for hatch_jupyter_builder."""
 import importlib
 import logging
 import os
 import shlex
 import subprocess
 import sys
 from pathlib import Path
@@ -9,22 +10,23 @@
 from typing import Any, Callable, Dict, List, Mapping, Optional, Union
 
 if sys.platform == "win32":  # pragma: no cover
     from subprocess import list2cmdline
 else:
 
     def list2cmdline(cmd_list):
+        """Implementation of list2cmdline for posix systems."""
         return " ".join(map(shlex.quote, cmd_list))
 
 
 _logger = None
 
 
 def _get_log() -> logging.Logger:
-    global _logger
+    global _logger  # noqa
     if _logger:
         return _logger
     _logger = logging.getLogger(__name__)
     _logger.setLevel(logging.INFO)
     logging.basicConfig(level=logging.INFO)
     return _logger
 
@@ -93,31 +95,28 @@
     # Find a suitable default for the npm command.
     if npm is None:
         is_yarn = (abs_path / "yarn.lock").exists()
         if is_yarn and not which("yarn"):
             log.warning("yarn not found, ignoring yarn.lock file")
             is_yarn = False
 
-        if is_yarn:
-            npm = ["yarn"]
-        else:
-            npm = ["npm"]
+        npm = ["yarn"] if is_yarn else ["npm"]
 
     npm_cmd = normalize_cmd(npm)
 
     if build_dir and source_dir and not force:
         should_build = is_stale(build_dir, source_dir)
     else:
         should_build = True
 
     if should_build:
         log.info("Installing build dependencies with npm.  This may take a while...")
-        run(npm_cmd + ["install"], cwd=str(abs_path))
+        run([*npm_cmd, "install"], cwd=str(abs_path))
         if build_cmd:
-            run(npm_cmd + ["run", build_cmd], cwd=str(abs_path))
+            run([*npm_cmd, "run", build_cmd], cwd=str(abs_path))
     else:
         log.info("No build required")
 
 
 def is_stale(target: Union[str, Path], source: Union[str, Path]) -> bool:
     """Test whether the target file/directory is stale based on the source
     file/directory.
@@ -175,49 +174,52 @@
 
 def mtime(path: Union[str, Path]) -> float:
     """shorthand for mtime"""
     return Path(path).stat().st_mtime
 
 
 def get_build_func(build_func_str: str) -> Callable[..., None]:
+    """Get a build function by name."""
     # Get the build function by importing it.
     mod_name, _, func_name = build_func_str.rpartition(".")
 
     # If the module fails to import, try importing as a local script.
     try:
         sys.path.insert(0, str(Path.cwd()))
         mod = importlib.import_module(mod_name)
     finally:
         sys.path.pop(0)
 
     return getattr(mod, func_name)
 
 
 def normalize_cmd(cmd: Union[str, list]) -> List[str]:
+    """Normalize a subprocess command."""
     if not isinstance(cmd, (list, tuple)):
         cmd = shlex.split(cmd, posix=os.name != "nt")
     if not Path(cmd[0]).is_absolute():
         # If a command is not an absolute path find it first.
         cmd_path = which(cmd[0])
         if not cmd_path:
-            raise ValueError(
+            msg = (
                 f"Aborting. Could not find cmd ({cmd[0]}) in path. "
                 "If command is not expected to be in user's path, "
                 "use an absolute path."
             )
+            raise ValueError(msg)
         cmd[0] = cmd_path
     return cmd
 
 
 def normalize_kwargs(kwargs: Mapping[str, str]) -> Dict[str, Any]:
     """Normalize the key names in a kwargs input dictionary"""
     result = {}
     for key, value in kwargs.items():
         if isinstance(value, bool):
-            value = str(value)
+            value = str(value)  # noqa
         result[key.replace("-", "_")] = value
     return result
 
 
 def run(cmd: Union[str, list], **kwargs: Any) -> int:
     """Echo a command before running it."""
     kwargs.setdefault("shell", os.name == "nt")
@@ -227,26 +229,28 @@
     return subprocess.check_call(cmd, **kwargs)
 
 
 def ensure_targets(ensured_targets: List[str]) -> None:
     """Ensure that target files are available"""
     for target in ensured_targets:
         if not Path(target).exists():
-            raise ValueError(f'Ensured target "{target}" does not exist')
+            msg = f'Ensured target "{target}" does not exist'
+            raise ValueError(msg)
     _get_log().info("Ensured target(s) exist!")
 
 
 def should_skip(skip_if_exists):
     """Detect whether all the paths in skip_if_exists exist"""
     if not isinstance(skip_if_exists, list) or not len(skip_if_exists):
         return False
     return all(os.path.exists(p) for p in skip_if_exists)
 
 
 def install_pre_commit_hook():
+    """Install a pre-commit hook."""
     data = f"""#!/usr/bin/env bash
 INSTALL_PYTHON={sys.executable}
 ARGS=(hook-impl --config=.pre-commit-config.yaml --hook-type=pre-commit)
 HERE="$(cd "$(dirname "$0")" && pwd)"
 ARGS+=(--hook-dir "$HERE" -- "$@")
 exec "$INSTALL_PYTHON" -m pre_commit "${{ARGS[@]}}"
 """
```

### Comparing `hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/compare_migrated/cli.py` & `hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/compare_migrated/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,46 +8,51 @@
 import sys
 import tarfile
 import zipfile
 from typing import Optional
 
 
 def build_file(dirname, dist_name):
+    """Build a dist file in a directory."""
     orig_dir = os.getcwd()
     os.chdir(dirname)
     if os.path.exists("dist"):
         shutil.rmtree("dist")
     subprocess.check_call([sys.executable, "-m", "build", f"--{dist_name}"])
     os.chdir(orig_dir)
 
 
 def get_tar_names(dirname):
+    """Get the tarball names in a directory."""
     dist_file = glob.glob(f"{dirname}/dist/*.tar.gz")[0]
     tarf = tarfile.open(dist_file, "r:gz")
     return set(tarf.getnames())
 
 
 def get_zip_names(dirname):
+    """Get the zip (wheel) file names in a directory."""
     wheel_file = glob.glob(f"{dirname}/dist/*.whl")[0]
     with zipfile.ZipFile(wheel_file, "r") as f:
         return set(f.namelist())
 
 
 def filter_file(path):
+    """Filter a file path for interesting files."""
     if "egg-info" in path:
         return True
     _, ext = os.path.splitext(path)
     if not ext:
         return True
     if os.path.basename(path) in [path, "setup.py", "setup.cfg", "MANIFEST.in"]:
         return True
     return False
 
 
 def main(source_dir, target_dir, dist_name):
+    """The main script."""
     subprocess.check_call([sys.executable, "-m", "pip", "install", "build"])
 
     logger = logging.getLogger(__name__)
     logging.basicConfig()
 
     build_file(source_dir, dist_name)
     build_file(target_dir, dist_name)
@@ -75,20 +80,22 @@
 
     return {"added": added, "removed": removed}
 
 
 def make_parser(
     parser: Optional[argparse.ArgumentParser] = None, prog: Optional[str] = None
 ) -> argparse.ArgumentParser:
+    """Make an arg parser."""
     if parser is None:
         parser = argparse.ArgumentParser(prog=prog)
     parser.add_argument(dest="source_dir", help="Source Directory")
     parser.add_argument(dest="target_dir", help="Target Directory")
     parser.add_argument(dest="dist_name", help="Dist name")
     return parser
 
 
 def run(args: Optional[argparse.Namespace] = None) -> None:
+    """Run the cli."""
     if args is None:
         parser = make_parser(prog=f"{sys.executable} -m hatch_jupyter_builder.compare_migrated")
         args = parser.parse_args()
     main(args.source_dir, args.target_dir, args.dist_name)
```

### Comparing `hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/migrate/_migrate.py` & `hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/migrate/_migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Handle migration."""
 import json
 import logging
 import os
 import subprocess
 import sys
 from pathlib import Path
 
@@ -29,15 +30,15 @@
 
 # Read pyproject before migration to get old build requirements.
 pyproject = Path("pyproject.toml")
 if pyproject.exists():
     data = tomli.loads(pyproject.read_text("utf-8"))
     requires = data["build-system"]["requires"]
     # Install the old build reqs into this venv.
-    subprocess.run([sys.executable, "-m", "pip", "install"] + requires)
+    subprocess.run([sys.executable, "-m", "pip", "install", *requires])
     requires = [
         r
         for r in requires
         if not r.startswith("jupyter-packaging")
         and not r.startswith("setuptools")
         and not r.startswith("jupyter_packaging")
         and not r.startswith("wheel")
@@ -151,17 +152,16 @@
     for option in ["ensured-targets", "skip-if-exists"]:
         if option in options_table:
             builder_table[option] = options_table[option]
 
     if build_args_table:
         builder_table["build-kwargs"] = build_args_table.copy()
 
-    if build_args_table.get("npm"):
-        if "editable-build-kwargs" in builder_table:
-            builder_table["editable-build-kwargs"]["npm"] = build_args_table["npm"]
+    if build_args_table.get("npm") and "editable-build-kwargs" in builder_table:
+        builder_table["editable-build-kwargs"]["npm"] = build_args_table["npm"]
 
 # Add artifacts config for package data that would be ignored.
 project_name = data.get("project", {}).get("name", "")
 gitignore = Path(".gitignore")
 artifacts = []
 if gitignore.exists() and project_name and Path(project_name).exists():
     text = gitignore.read_text("utf-8")
```

### Comparing `hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/migrate/cli.py` & `hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/migrate/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,21 +10,19 @@
 from tempfile import TemporaryDirectory
 from typing import Optional
 
 from hatch_jupyter_builder import __version__ as builder_version
 
 
 def main(td, target_dir):
+    """Main script."""
     logger = logging.getLogger(__name__)
     logging.basicConfig()
     venv.create(td, with_pip=True)
-    if os.name == "nt":
-        python = Path(td) / "Scripts/python.exe"
-    else:
-        python = Path(td) / "bin/python"
+    python = Path(td) / "Scripts/python.exe" if os.name == "nt" else Path(td) / "bin/python"
 
     logger.info("Installing in temporary virtual environment...")
 
     # Create a virtual environment and use it to run the migration.
     runner = subprocess.check_call
     runner([python, "-m", "pip", "install", "build"])
     runner([python, "-m", "pip", "install", "packaging"])
@@ -36,19 +34,21 @@
     migrator = Path(__file__).parent / "_migrate.py"
     runner([python, migrator, builder_version], cwd=target_dir)
 
 
 def make_parser(
     parser: Optional[argparse.ArgumentParser] = None, prog: Optional[str] = None
 ) -> argparse.ArgumentParser:
+    """Make a parser object."""
     if parser is None:
         parser = argparse.ArgumentParser(prog=prog)
     parser.add_argument(dest="target_dir", help="Target Directory")
     return parser
 
 
 def run(args: Optional[argparse.Namespace] = None) -> None:
+    """Run the migration."""
     if args is None:
         parser = make_parser(prog=f"{sys.executable} -m hatch_jupyter_builder.migrate")
         args = parser.parse_args()
     with TemporaryDirectory() as td:
         main(td, args.target_dir)
```

### Comparing `hatch_jupyter_builder-0.8.2/hatch_jupyter_builder/migrate/jupyter_packaging.py` & `hatch_jupyter_builder-0.8.3/hatch_jupyter_builder/migrate/jupyter_packaging.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Shim for jupyter packaging migration."""
 import os
 import sys
 from pathlib import Path
 
 import tomli
 import tomli_w
 
@@ -53,35 +54,38 @@
             build_kwargs[name] = value
     if kwargs.get("force"):
         build_kwargs["force"] = True
     return build_kwargs
 
 
 def skip_if_exists(paths, *args):
+    """Shim for skip if exists"""
     if paths:
         data = {"skip-if-exists": [_normalize_path(p) for p in paths]}
         _write_config("tool.hatch.build.hooks.jupyter-builder", data)
     return __real_jupyter_packaging.skip_if_exists(paths, *args)
 
 
 def ensure_targets(targets):
+    """Shim for ensure targets"""
     if targets:
         data = {"ensured-targets": [_normalize_path(t) for t in targets]}
         _write_config("tool.hatch.build.hooks.jupyter-builder", data)
     return __real_jupyter_packaging.ensure_targets(targets)
 
 
 def wrap_installers(
     pre_develop=None,
     pre_dist=None,
     post_develop=None,
     post_dist=None,
     ensured_targets=None,
     skip_if_exists=None,
 ):
+    """Shim for wrap_installers."""
     if pre_develop or post_develop:
         func = pre_develop or post_develop
         build_kwargs = _get_build_kwargs(**func.__kwargs)
         _write_config("tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs", build_kwargs)
 
     if pre_dist or post_dist:
         func = pre_dist or post_dist
@@ -101,19 +105,20 @@
         skip_if_exists=skip_if_exists,
     )
 
 
 def create_cmdclass(
     prerelease_cmd=None, package_data_spec=None, data_files_spec=None, exclude=None
 ):
+    """Shim for create_cmdclass."""
     shared_data = {}
     if data_files_spec is not None:
-        for (path, dname, pattern) in data_files_spec:
+        for path, dname, pattern in data_files_spec:
             if os.path.isabs(dname):
-                dname = os.path.relpath(dname, os.getcwd())
+                dname = os.path.relpath(dname, os.getcwd())  # noqa
             if pattern == "**":
                 shared_data[dname] = path
             else:
                 shared_data[f"{dname}/{pattern}"] = f"{path}/{pattern}"
 
     _write_config("tool.hatch.build.targets.wheel.shared-data", shared_data)
 
@@ -124,14 +129,15 @@
         exclude=exclude,
     )
 
 
 def install_npm(
     path=None, build_dir=None, source_dir=None, build_cmd="build", force=False, npm=None
 ):
+    """Shim for install_npm."""
     build_kwargs = _get_build_kwargs(**locals())
     if build_kwargs:
         _write_config("tool.hatch.build.hooks.jupyter-builder.build-kwargs", build_kwargs)
 
     return __real_jupyter_packaging.install_npm(
         path=path,
         build_dir=build_dir,
@@ -141,27 +147,29 @@
         npm=npm,
     )
 
 
 def npm_builder(
     path=None, build_dir=None, source_dir=None, build_cmd="build", force=False, npm=None
 ):
+    """Shim for npm_builder."""
     func = __real_jupyter_packaging.npm_builder(
         path=path,
         build_dir=build_dir,
         source_dir=source_dir,
         build_cmd=build_cmd,
         force=force,
         npm=npm,
     )
     func.__kwargs = {}
-    for name in _npm_kwargs + ["force"]:
+    for name in [*_npm_kwargs, "force"]:
         func.__kwargs[name] = locals()[name]
     return func
 
 
 def __getattr__(name):
+    """Defer to the original for all others."""
     return getattr(__real_jupyter_packaging, name)
 
 
 del __this_shim
 del __current_directory
```

### Comparing `hatch_jupyter_builder-0.8.2/tests/conftest.py` & `hatch_jupyter_builder-0.8.3/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,12 +17,11 @@
 
 def pytest_runtest_setup(item):
     is_migration_test = any(mark for mark in item.iter_markers(name="migration_test"))
 
     if item.config.getoption("--migration-tests") is True:
         if not is_migration_test:
             pytest.skip("Only running tests marked as 'migration_test'.")
-    else:
-        if is_migration_test:
-            pytest.skip(
-                "Skipping this test because it's marked 'migration_test'. Run integration tests using the `--migration-tests` flag."
-            )
+    elif is_migration_test:
+        pytest.skip(
+            "Skipping this test because it's marked 'migration_test'. Run integration tests using the `--migration-tests` flag."
+        )
```

### Comparing `hatch_jupyter_builder-0.8.2/tests/test_is_stale.py` & `hatch_jupyter_builder-0.8.3/tests/test_is_stale.py`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/test_migration.py` & `hatch_jupyter_builder-0.8.3/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/test_npm_builder.py` & `hatch_jupyter_builder-0.8.3/tests/test_npm_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     run = mocker.patch("hatch_jupyter_builder.utils.run")
     os.environ["HATCH_JUPYTER_BUILDER_SKIP_NPM"] = "1"
     which.return_value = "foo"
     npm_builder("wheel", "standard", path=repo)
     run.assert_not_called()
     del os.environ["HATCH_JUPYTER_BUILDER_SKIP_NPM"]
 
-    sys.argv = sys.argv + ["--skip-npm"]
+    sys.argv = [*sys.argv, "--skip-npm"]
     npm_builder("wheel", "standard", path=repo)
     run.assert_not_called()
 
 
 def test_npm_builder_yarn(mocker, repo):
     which = mocker.patch("hatch_jupyter_builder.utils.which")
     run = mocker.patch("hatch_jupyter_builder.utils.run")
```

### Comparing `hatch_jupyter_builder-0.8.2/tests/test_plugin.py` & `hatch_jupyter_builder-0.8.3/tests/test_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,24 @@
 import subprocess
 import sys
 import venv
 import warnings
 from pathlib import Path
 
 import pytest
+from hatchling.metadata.core import ProjectMetadata
+from hatchling.plugin.manager import PluginManager
 
 from hatch_jupyter_builder.plugin import JupyterBuildHook
 
 
 def test_build_hook(tmp_path):
+    manager = PluginManager()
+    meta = ProjectMetadata(".", manager, {})
+
     if "SKIP_JUPYTER_BUILD" in os.environ:
         del os.environ["SKIP_JUPYTER_BUILD"]
 
     config = {
         "build-function": "test.foo",
         "ensured-targets": ["test.py"],
         "build-kwargs": {"foo-bar": "1", "fizz_buzz": "2"},
@@ -26,59 +31,59 @@
     text = """
 def foo(target_name, version, foo_bar=None, fizz_buzz=None):
     return(target_name)
 """
     test.write_text(text, encoding="utf-8")
     os.makedirs(".git/hooks")
 
-    hook = JupyterBuildHook(tmp_path, config, {}, {}, tmp_path, "wheel")
+    hook = JupyterBuildHook(tmp_path, config, {}, meta, tmp_path, "wheel")
     assert hook.initialize("standard", {})
     assert hook.initialize("editable", {})
 
-    hook = JupyterBuildHook(tmp_path, config, {}, {}, tmp_path, "sdist")
+    hook = JupyterBuildHook(tmp_path, config, {}, meta, tmp_path, "sdist")
     assert hook.initialize("standard", {})
 
-    hook = JupyterBuildHook(tmp_path, {}, {}, {}, tmp_path, "wheel")
+    hook = JupyterBuildHook(tmp_path, {}, {}, meta, tmp_path, "wheel")
     assert hook.initialize("standard", {})
     assert hook.initialize("editable", {})
 
     config["skip-if-exists"] = ["foo", "bar"]
     assert hook.initialize("standard", {})
     del config["skip-if-exists"]
 
     config["editable-build-kwargs"] = {"foo-bar": "2", "fizz_buzz": "3"}
     assert hook.initialize("editable", {})
 
-    hook = JupyterBuildHook(tmp_path, config, {}, {}, tmp_path, "foo")
+    hook = JupyterBuildHook(tmp_path, config, {}, meta, tmp_path, "foo")
     assert not hook.initialize("standard", {})
 
     text = """
 def foo(target_name, version, foo_bar=None, fizz_buzz=None):
     raise RuntimeError('trigger error')
 """
     test.write_text(text, encoding="utf-8")
     # Force a re-import
     del sys.modules["test"]
 
-    hook = JupyterBuildHook(tmp_path, config, {}, {}, tmp_path, "wheel")
+    hook = JupyterBuildHook(tmp_path, config, {}, meta, tmp_path, "wheel")
     with pytest.raises(RuntimeError):
         hook.initialize("editable", {})
 
     os.environ["SKIP_JUPYTER_BUILDER"] = "1"
     assert not hook.initialize("standard", {})
     del os.environ["SKIP_JUPYTER_BUILDER"]
 
     config["optional-editable-build"] = "true"
-    hook = JupyterBuildHook(tmp_path, config, {}, {}, tmp_path, "wheel")
+    hook = JupyterBuildHook(tmp_path, config, {}, meta, tmp_path, "wheel")
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         assert hook.initialize("editable", {})
 
     config["optional-editable-build"] = True
-    hook = JupyterBuildHook(tmp_path, config, {}, {}, tmp_path, "wheel")
+    hook = JupyterBuildHook(tmp_path, config, {}, meta, tmp_path, "wheel")
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         assert hook.initialize("editable", {})
 
     del sys.modules["test"]
```

### Comparing `hatch_jupyter_builder-0.8.2/tests/test_utils.py` & `hatch_jupyter_builder-0.8.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/pyproject.toml` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/.eslintrc.js` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/.gitignore` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/LICENSE.txt` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/MANIFEST.in` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/README.md` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/README.md`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/package.json` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/package.json`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/setup.py` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/setup.py`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/tsconfig.json` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/tsconfig.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666666%*

 * *Differences: {"'compilerOptions'": "{'target': 'es2018'}"}*

```diff
@@ -13,15 +13,15 @@
         "outDir": "lib",
         "resolveJsonModule": true,
         "rootDir": "src",
         "skipLibCheck": true,
         "sourceMap": true,
         "strict": true,
         "strictPropertyInitialization": false,
-        "target": "es2015",
+        "target": "es2018",
         "types": [
             "jest"
         ]
     },
     "exclude": [
         "src/**/__tests__"
     ],
```

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/webpack.config.js` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/webpack.config.js`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/.github/workflows/build.yml` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/Makefile` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/make.bat` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/source/conf.py` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/source/develop-install.rst` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/source/index.rst` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/docs/source/installing.rst` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/examples/introduction.ipynb` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/examples/introduction.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996875%*

 * *Differences: {"'cells'": '{3: {\'source\': [\'assert w.value == "Hello World"\']}}'}*

```diff
@@ -28,15 +28,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert w.value == 'Hello World'"
+                "assert w.value == \"Hello World\""
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject/__init__.py` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject/example.py` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject/example.py`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/myproject/tests/conftest.py` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/myproject/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/extension.ts` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/extension.ts`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/plugin.ts` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/version.ts` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/version.ts`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/widget.ts` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/widget.ts`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/__tests__/index.spec.ts` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/create_cmdclass/myproject/src/__tests__/utils.ts` & `hatch_jupyter_builder-0.8.3/tests/data/create_cmdclass/myproject/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/pyproject.toml` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/.eslintrc.js` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/.gitignore` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/LICENSE` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/README.md` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/README.md`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/RELEASE.md` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/RELEASE.md`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/package.json` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/package.json`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/pyproject.toml` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/setup.py` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/setup.py`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/tsconfig.json` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/tsconfig.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'compilerOptions'": "{'target': 'es2018'}"}*

```diff
@@ -13,14 +13,14 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2017",
+        "target": "es2018",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/.github/workflows/build.yml` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/.github/workflows/check-release.yml` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/myextension/_version.py` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/myextension/_version.py`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/tests/data/npm_builder/myextension/src/index.ts` & `hatch_jupyter_builder-0.8.3/tests/data/npm_builder/myextension/src/index.ts`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/LICENSE.txt` & `hatch_jupyter_builder-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_jupyter_builder-0.8.2/README.md` & `hatch_jupyter_builder-0.8.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # hatch-jupyter-builder
 
 [![PyPI - Version](https://img.shields.io/pypi/v/hatch-jupyter-builder.svg)](https://pypi.org/project/hatch-jupyter-builder)
-[![codecov](https://codecov.io/gh/jupyterlab/hatch-jupyter-builder/branch/master/graph/badge.svg?token=DrOulNuIzL)](https://codecov.io/gh/jupyterlab/hatch-jupyter-builder)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 
 ______________________________________________________________________
 
 This provides a [build hook](https://hatch.pypa.io/latest/config/build/#build-hooks) plugin for [Hatch](https://github.com/pypa/hatch) that adds a build step for use with Jupyter packages.
 
 **Table of Contents**
```

### Comparing `hatch_jupyter_builder-0.8.2/pyproject.toml` & `hatch_jupyter_builder-0.8.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 license = { file = "LICENSE.txt" }
 keywords = ["jupyter", "jupyterlab", "hatch"]
 authors = [
   { name = "Jupyter Development Team", email = "jupyter@googlegroups.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
+  "License :: OSI Approved :: BSD License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
@@ -28,29 +29,32 @@
 [project.urls]
 Documentation = "https://github.com/jupyterlab/hatch-jupyter-builder#readme"
 Issues = "https://github.com/jupyterlab/hatch-jupyter-builder/issues"
 Source = "https://github.com/jupyterlab/hatch-jupyter-builder"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-mock", "hatch", "pytest-cov", "tomli", "twine"]
-docs = ["pydata-sphinx-theme", "myst-parser", "hatch_jupyter_builder"]
+docs = ["pydata-sphinx-theme", "myst-parser", "hatch_jupyter_builder", "sphinxcontrib-spelling", "sphinx-autodoc-typehints"]
 
 [project.scripts]
 hatch-jupyter-builder = 'hatch_jupyter_builder.cli:run'
 
 [project.entry-points.hatch]
 jupyter = "hatch_jupyter_builder.hooks"
 
 [tool.hatch.version]
 path = "hatch_jupyter_builder/__init__.py"
 
 [tool.hatch.envs.docs]
 features = ["docs"]
+[tool.hatch.envs.docs.env-vars]
+SPHINXOPTS = "-W"
 [tool.hatch.envs.docs.scripts]
-build = "make -C docs html SPHINXOPTS='-W'"
+build = "make -C docs html"
+api = "sphinx-apidoc -o docs/source/reference/api -f -E hatch_jupyter_builder hatch_jupyter_builder/migrate/jupyter_packaging.py"
 
 [tool.hatch.envs.test]
 features = ["test"]
 [tool.hatch.envs.test.scripts]
 test = "python -m pytest -vv {args}"
 nowarn = "python -m pytest -vv -W default {args}"
 
@@ -70,17 +74,17 @@
 features = ["test"]
 dependencies = ["mypy>=0.990"]
 [tool.hatch.envs.typing.scripts]
 test = "mypy --install-types --non-interactive {args:hatch_jupyter_builder/**/*.py tests/*.py}"
 
 [tool.hatch.envs.lint]
 dependencies = [
-  "black>=22.6.0",
+  "black[jupyter]==23.3.0",
   "mdformat>0.7",
-  "ruff==0.0.177",
+  "ruff==0.0.260",
 ]
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:docs/source *.md}"
 ]
@@ -102,14 +106,16 @@
 
 [tool.coverage.run]
 omit = [
    "hatch_jupyter_builder/cli.py",
    "hatch_jupyter_builder/migrate/*",
    "hatch_jupyter_builder/compare_migrated/*"
 ]
+relative_files = true
+source = ["hatch_jupyter_builder"]
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_incomplete_defs = true
 no_implicit_optional = true
 pretty = true
 show_error_context = true
@@ -124,16 +130,17 @@
 line-length = 100
 target-version = ["py38"]
 
 [tool.ruff]
 target-version = "py38"
 line-length = 100
 select = [
-  "A", "B", "C", "E", "F", "FBT", "I", "N", "Q", "RUF", "S", "T",
-  "UP", "W", "YTT",
+  "A", "B", "C", "DTZ", "E", "EM", "F", "FBT", "I", "ICN", "ISC", "N",
+  "PLC", "PLE", "PLR", "PLW", "Q", "RUF", "S", "SIM", "T", "TID", "UP",
+  "W", "YTT",
 ]
 ignore = [
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Ignore McCabe complexity
   "C901",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
@@ -156,14 +163,20 @@
   # Possible hardcoded password
   "S105",
   "S106",
   # Variable `xxx` in function should be lowercase
   "N806",
   # Exception name `KernelSessionRecordConflict` should be named with an Error suffix
   "N818",
+  # SIM105 Use `contextlib.suppress(...)`
+  "SIM105",
+  # PLR0913 Too many arguments to function call
+  "PLR0913",
+  # PLR0912 Too many branches
+  "PLR0912",
 ]
 unfixable = [
   # Don't touch print statements
   "T201",
   # Don't touch unused imports
   "F401",
   # Don't touch noqa lines
@@ -172,8 +185,20 @@
 
 [tool.ruff.per-file-ignores]
 # B011 Do not call assert False since python -O removes these calls
 # F841 local variable 'foo' is assigned to but never used
 # C408 Unnecessary `dict` call
 # E402 Module level import not at top of file
 # T201 `print` found
-"tests/*" = ["B011", "F841", "C408", "E402", "T201"]
+# EM101 Exception must not use a string literal
+# PLR2004 Magic value used in comparison
+"tests/*" = ["B011", "F841", "C408", "E402", "T201", "EM101", "EM102", "EM103", "PLR2004"]
+
+[tool.interrogate]
+ignore-init-module=true
+ignore-private=true
+ignore-semiprivate=true
+ignore-property-decorators=true
+ignore-nested-functions=true
+ignore-nested-classes=true
+fail-under=100
+exclude = ["docs", "tests"]
```

### Comparing `hatch_jupyter_builder-0.8.2/PKG-INFO` & `hatch_jupyter_builder-0.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-jupyter-builder
-Version: 0.8.2
+Version: 0.8.3
 Summary: A hatch plugin to help build Jupyter packages
 Project-URL: Documentation, https://github.com/jupyterlab/hatch-jupyter-builder#readme
 Project-URL: Issues, https://github.com/jupyterlab/hatch-jupyter-builder/issues
 Project-URL: Source, https://github.com/jupyterlab/hatch-jupyter-builder
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: Copyright (c) 2022 Project Jupyter Contributors
         All rights reserved.
@@ -32,40 +32,42 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE.txt
 Keywords: hatch,jupyter,jupyterlab
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: hatchling>=1.5
 Provides-Extra: docs
 Requires-Dist: hatch-jupyter-builder; extra == 'docs'
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
+Requires-Dist: sphinxcontrib-spelling; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: hatch; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-mock; extra == 'test'
 Requires-Dist: tomli; extra == 'test'
 Requires-Dist: twine; extra == 'test'
 Description-Content-Type: text/markdown
 
 # hatch-jupyter-builder
 
 [![PyPI - Version](https://img.shields.io/pypi/v/hatch-jupyter-builder.svg)](https://pypi.org/project/hatch-jupyter-builder)
-[![codecov](https://codecov.io/gh/jupyterlab/hatch-jupyter-builder/branch/master/graph/badge.svg?token=DrOulNuIzL)](https://codecov.io/gh/jupyterlab/hatch-jupyter-builder)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 
 ______________________________________________________________________
 
 This provides a [build hook](https://hatch.pypa.io/latest/config/build/#build-hooks) plugin for [Hatch](https://github.com/pypa/hatch) that adds a build step for use with Jupyter packages.
 
 **Table of Contents**
```

