# Comparing `tmp/bo4e-202401.1.0rc1.tar.gz` & `tmp/bo4e-202401.1.0rc2.tar.gz`

## Comparing `bo4e-202401.1.0rc1.tar` & `bo4e-202401.1.0rc2.tar`

### file list

```diff
@@ -1,338 +1,338 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.pylintrc
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.readthedocs.yaml
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/CHANGELOG.rst
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/MANIFEST.in
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/README.rst
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/bo4e_schemas_create_release.py
--rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/generate_or_validate_json_schemas.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/requirements.in
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/requirements.txt
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tox.ini
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.github/dependabot.yml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.github/workflows/linting.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.github/workflows/python-publish-scheduled.yml
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.vscode/settings.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-json_schemas.in
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-json_schemas.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/Makefile
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/authors.rst
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/changelog.rst
--rw-r--r--   0        0        0    11053 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/conf.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/index.rst
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/license.rst
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/release_workflow.rst
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/requirements.in
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/requirements.txt
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/test_uml.py
--rw-r--r--   0        0        0    28433 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/uml.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/versioning.rst
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/_static/bo4e-python-favicon.png
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/_static/bo4e-python-favicon.svg
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/_static/bo4e-python-logo.png
--rw-r--r--   0        0        0    26543 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/_static/bo4e-python-logo.svg
--rw-r--r--   0        0        0   167661 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/_static/bo4e-release-workflow.excalidraw
--rw-r--r--   0        0        0   512116 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/docs/_static/bo4e-release-workflow.png
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/_bo4e_python_version.py
--rw-r--r--   0        0        0    12614 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/py.typed
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/version.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/zusatzattribut.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/__init__.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/angebot.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/ausschreibung.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/buendelvertrag.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/energiemenge.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/fremdkosten.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/geraet.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/geschaeftsobjekt.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/geschaeftspartner.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/kosten.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/lastgang.py
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/marktlokation.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/marktteilnehmer.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/messlokation.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/person.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/preisblatt.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/preisblattdienstleistung.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/preisblatthardware.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/preisblattkonzessionsabgabe.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/preisblattmessung.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/preisblattnetznutzung.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/rechnung.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/region.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/regionaltarif.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/standorteigenschaften.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/tarif.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/tarifinfo.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/tarifkosten.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/tarifpreisblatt.py
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/vertrag.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/zaehler.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/bo/zeitreihe.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/adresse.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/angebotsposition.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/angebotsteil.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/angebotsvariante.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/aufabschlag.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/aufabschlagproort.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/aufabschlagregional.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/aufabschlagstaffelproort.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/ausschreibungsdetail.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/ausschreibungslos.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/betrag.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/com.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/dienstleistung.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/energieherkunft.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/energiemix.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/fremdkostenblock.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/fremdkostenposition.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/geokoordinaten.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/katasteradresse.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/kontaktweg.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/konzessionsabgabe.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/kostenblock.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/kostenposition.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/kriteriumwert.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/marktgebietinfo.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/menge.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/messlokationszuordnung.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/positionsaufabschlag.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/preis.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/preisgarantie.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/preisposition.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/preisstaffel.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/rechnungsposition.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/regionalegueltigkeit.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/regionalepreisgarantie.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/regionalepreisstaffel.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/regionaleraufabschlag.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/regionaletarifpreisposition.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/regionskriterium.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/sigmoidparameter.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/standorteigenschaftengas.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/standorteigenschaftenstrom.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/steuerbetrag.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/tarifberechnungsparameter.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/tarifeinschraenkung.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/tarifpreis.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/tarifpreisposition.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/tarifpreispositionproort.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/tarifpreisstaffelproort.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/unterschrift.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/verbrauch.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/vertragskonditionen.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/vertragsteil.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/verwendungszweckpromarktrolle.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/zaehlwerk.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/zaehlzeitregister.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/zeitraum.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/zeitreihenwert.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/zeitspanne.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/com/zustaendigkeit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/__init__.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/abgabeart.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/angebotsstatus.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/anrede.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/arithmetische_operation.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/artikelid.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/aufabschlagstyp.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/aufabschlagsziel.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/ausschreibungsportal.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/ausschreibungsstatus.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/ausschreibungstyp.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/bdewartikelnummer.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/befestigungsart.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/bemessungsgroesse.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/bilanzierungsmethode.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/dienstleistungstyp.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/energierichtung.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/erzeugungsart.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/gasqualitaet.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/gebiettyp.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/geraeteklasse.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/geraetetyp.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/geschaeftspartnerrolle.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/gueltigkeitstyp.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/kalkulationsmethode.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/kontaktart.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/kostenklasse.py
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/kundengruppe.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/kundengruppeka.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/kundentyp.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/landescode.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/leistungstyp.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/lokationstyp.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/marktrolle.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/medium.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/mengeneinheit.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/mengenoperator.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/messart.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/messgroesse.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/messpreistyp.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/messwerterfassung.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/messwertstatus.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/messwertstatuszusatz.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/netzebene.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/netznutzungrechnungsart.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/netznutzungrechnungstyp.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/oekolabel.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/oekozertifikat.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/organisationstyp.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/preisgarantietyp.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/preismodell.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/preisstatus.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/preistyp.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/rechnungslegung.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/rechnungsstatus.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/rechnungstyp.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/regionskriteriumtyp.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/registeranzahl.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/rollencodetyp.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/sparte.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/steuerkennzeichen.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/strenum.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/tarifkalkulationsmethode.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/tarifmerkmal.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/tarifregionskriterium.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/tariftyp.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/tarifzeit.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/themengebiet.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/titel.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/typ.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/verbrauchsart.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/vertragsart.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/vertragsform.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/vertragsstatus.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/verwendungszweck.py
--rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/voraussetzungen.py
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/waehrungscode.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/waehrungseinheit.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/waermenutzung.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/wertermittlungsverfahren.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/zaehlerauspraegung.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/zaehlergroesse.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/zaehlertyp.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/enum/zaehlertypspezifikation.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/src/bo4e/utils/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/__init__.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/serialization_helper.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_adresse.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_angebot.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_angebotsposition.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_angebotsteil.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_angebotsvariante.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_aufabschlag.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_aufabschlagproort.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_aufabschlagregional.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_aufabschlagstaffelproort.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_ausschreibung.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_ausschreibungsdetail.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_ausschreibungslos.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_betrag.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_buendelvertrag.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_energieherkunft.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_energiemenge.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_energiemix.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_enums.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_fremdkosten.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_fremdkostenblock.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_fremdkostenposition.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_geokoordinaten.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_geraet.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_geschaeftsobjekt.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_geschaeftspartner.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_import_enum.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_katasteradresse.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_kontakt.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_kosten.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_kostenblock.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_kostenposition.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_kriteriumswert.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_lastgang.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_marktgebietinfo.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_marktlokation.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_marktteilnehmer.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_menge.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_messlokation.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_messlokationszuordnung.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_person.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_positionsaufabschlag.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_preis.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_preisblatt.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_preisblatt_dienstleistung.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_preisblatt_hardware.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_preisblatt_konzessionsabgabe.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_preisblatt_messung.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_preisblattnetznutzung.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_preisgarantie.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_preisposition.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_preisstaffel.py
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_rechnung.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_rechnungsposition.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_region.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_regionalegueltigkeit.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_regionalepreisgarantie.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_regionalepreisstaffel.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_regionaleraufabschlag.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_regionaletarifpreisposition.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_regionaltarif.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_regionskriterium.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_sigmoidparameter.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_standorteigenschaften.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_standorteigenschaftengas.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_standorteigenschaftenstrom.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_steuerbetrag.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_tarif.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_tarifberechnungsparameter.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_tarifeinschraenkung.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_tarifinfo.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_tarifkosten.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_tarifpreis.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_tarifpreisblatt.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_tarifpreisposition.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_tarifpreispositionproort.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_tarifpreisstaffelproort.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_unterschrift.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_verbrauch.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_vertrag.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_vertragskonditionen.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_vertragsteil.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_zaehler.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_zeitraum.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_zeitreihe.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_zeitreihenwert.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_zeitspanne.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_zusatz_attribut.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/utils.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/.gitignore
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/AUTHORS.rst
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/LICENSE.rst
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.pylintrc
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.readthedocs.yaml
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/CHANGELOG.rst
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/MANIFEST.in
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/README.rst
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/bo4e_schemas_create_release.py
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/generate_or_validate_json_schemas.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/requirements.in
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/requirements.txt
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tox.ini
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/linting.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/python-publish-scheduled.yml
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.vscode/settings.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-json_schemas.in
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-json_schemas.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/Makefile
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/authors.rst
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/changelog.rst
+-rw-r--r--   0        0        0    11035 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/conf.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/index.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/license.rst
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/release_workflow.rst
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/requirements.in
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/requirements.txt
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/test_uml.py
+-rw-r--r--   0        0        0    28433 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/uml.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/versioning.rst
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/_static/bo4e-python-favicon.png
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/_static/bo4e-python-favicon.svg
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/_static/bo4e-python-logo.png
+-rw-r--r--   0        0        0    26543 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/_static/bo4e-python-logo.svg
+-rw-r--r--   0        0        0   167661 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/_static/bo4e-release-workflow.excalidraw
+-rw-r--r--   0        0        0   512116 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/docs/_static/bo4e-release-workflow.png
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/_bo4e_python_version.py
+-rw-r--r--   0        0        0    12614 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/py.typed
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/version.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/zusatzattribut.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/__init__.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/angebot.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/ausschreibung.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/buendelvertrag.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/energiemenge.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/fremdkosten.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/geraet.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/geschaeftsobjekt.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/geschaeftspartner.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/kosten.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/lastgang.py
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/marktlokation.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/marktteilnehmer.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/messlokation.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/person.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/preisblatt.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/preisblattdienstleistung.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/preisblatthardware.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/preisblattkonzessionsabgabe.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/preisblattmessung.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/preisblattnetznutzung.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/rechnung.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/region.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/regionaltarif.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/standorteigenschaften.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/tarif.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/tarifinfo.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/tarifkosten.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/tarifpreisblatt.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/vertrag.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/zaehler.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/bo/zeitreihe.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/adresse.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/angebotsposition.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/angebotsteil.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/angebotsvariante.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/aufabschlag.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/aufabschlagproort.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/aufabschlagregional.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/aufabschlagstaffelproort.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/ausschreibungsdetail.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/ausschreibungslos.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/betrag.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/com.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/dienstleistung.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/energieherkunft.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/energiemix.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/fremdkostenblock.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/fremdkostenposition.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/geokoordinaten.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/katasteradresse.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/kontaktweg.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/konzessionsabgabe.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/kostenblock.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/kostenposition.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/kriteriumwert.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/marktgebietinfo.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/menge.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/messlokationszuordnung.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/positionsaufabschlag.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/preis.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/preisgarantie.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/preisposition.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/preisstaffel.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/rechnungsposition.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/regionalegueltigkeit.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/regionalepreisgarantie.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/regionalepreisstaffel.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/regionaleraufabschlag.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/regionaletarifpreisposition.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/regionskriterium.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/sigmoidparameter.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/standorteigenschaftengas.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/standorteigenschaftenstrom.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/steuerbetrag.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/tarifberechnungsparameter.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/tarifeinschraenkung.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/tarifpreis.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/tarifpreisposition.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/tarifpreispositionproort.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/tarifpreisstaffelproort.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/unterschrift.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/verbrauch.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/vertragskonditionen.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/vertragsteil.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/verwendungszweckpromarktrolle.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/zaehlwerk.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/zaehlzeitregister.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/zeitraum.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/zeitreihenwert.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/zeitspanne.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/com/zustaendigkeit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/__init__.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/abgabeart.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/angebotsstatus.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/anrede.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/arithmetische_operation.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/artikelid.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/aufabschlagstyp.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/aufabschlagsziel.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/ausschreibungsportal.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/ausschreibungsstatus.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/ausschreibungstyp.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/bdewartikelnummer.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/befestigungsart.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/bemessungsgroesse.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/bilanzierungsmethode.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/dienstleistungstyp.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/energierichtung.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/erzeugungsart.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/gasqualitaet.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/gebiettyp.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/geraeteklasse.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/geraetetyp.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/geschaeftspartnerrolle.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/gueltigkeitstyp.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/kalkulationsmethode.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/kontaktart.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/kostenklasse.py
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/kundengruppe.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/kundengruppeka.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/kundentyp.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/landescode.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/leistungstyp.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/lokationstyp.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/marktrolle.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/medium.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/mengeneinheit.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/mengenoperator.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/messart.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/messgroesse.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/messpreistyp.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/messwerterfassung.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/messwertstatus.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/messwertstatuszusatz.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/netzebene.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/netznutzungrechnungsart.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/netznutzungrechnungstyp.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/oekolabel.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/oekozertifikat.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/organisationstyp.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/preisgarantietyp.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/preismodell.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/preisstatus.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/preistyp.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/rechnungslegung.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/rechnungsstatus.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/rechnungstyp.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/regionskriteriumtyp.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/registeranzahl.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/rollencodetyp.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/sparte.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/steuerkennzeichen.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/strenum.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/tarifkalkulationsmethode.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/tarifmerkmal.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/tarifregionskriterium.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/tariftyp.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/tarifzeit.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/themengebiet.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/titel.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/typ.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/verbrauchsart.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/vertragsart.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/vertragsform.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/vertragsstatus.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/verwendungszweck.py
+-rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/voraussetzungen.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/waehrungscode.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/waehrungseinheit.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/waermenutzung.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/wertermittlungsverfahren.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/zaehlerauspraegung.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/zaehlergroesse.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/zaehlertyp.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/enum/zaehlertypspezifikation.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/src/bo4e/utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/serialization_helper.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_adresse.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_angebot.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_angebotsposition.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_angebotsteil.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_angebotsvariante.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_aufabschlag.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_aufabschlagproort.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_aufabschlagregional.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_aufabschlagstaffelproort.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_ausschreibung.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_ausschreibungsdetail.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_ausschreibungslos.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_betrag.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_buendelvertrag.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_energieherkunft.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_energiemenge.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_energiemix.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_enums.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_fremdkosten.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_fremdkostenblock.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_fremdkostenposition.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_geokoordinaten.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_geraet.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_geschaeftsobjekt.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_geschaeftspartner.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_import_enum.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_katasteradresse.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_kontakt.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_kosten.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_kostenblock.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_kostenposition.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_kriteriumswert.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_lastgang.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_marktgebietinfo.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_marktlokation.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_marktteilnehmer.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_menge.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_messlokation.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_messlokationszuordnung.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_person.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_positionsaufabschlag.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preis.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisblatt.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisblatt_dienstleistung.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisblatt_hardware.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisblatt_konzessionsabgabe.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisblatt_messung.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisblattnetznutzung.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisgarantie.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisposition.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_preisstaffel.py
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_rechnung.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_rechnungsposition.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_region.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionalegueltigkeit.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionalepreisgarantie.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionalepreisstaffel.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionaleraufabschlag.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionaletarifpreisposition.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionaltarif.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_regionskriterium.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_sigmoidparameter.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_standorteigenschaften.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_standorteigenschaftengas.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_standorteigenschaftenstrom.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_steuerbetrag.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarif.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifberechnungsparameter.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifeinschraenkung.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifinfo.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifkosten.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifpreis.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifpreisblatt.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifpreisposition.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifpreispositionproort.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_tarifpreisstaffelproort.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_unterschrift.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_verbrauch.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_vertrag.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_vertragskonditionen.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_vertragsteil.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_zaehler.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_zeitraum.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_zeitreihe.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_zeitreihenwert.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_zeitspanne.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_zusatz_attribut.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/utils.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/.gitignore
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/AUTHORS.rst
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/LICENSE.rst
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 bo4e-202401.1.0rc2/PKG-INFO
```

### Comparing `bo4e-202401.1.0rc1/.pre-commit-config.yaml` & `bo4e-202401.1.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/.pylintrc` & `bo4e-202401.1.0rc2/.pylintrc`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/.readthedocs.yaml` & `bo4e-202401.1.0rc2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/CONTRIBUTING.md` & `bo4e-202401.1.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/README.rst` & `bo4e-202401.1.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/bo4e_schemas_create_release.py` & `bo4e-202401.1.0rc2/bo4e_schemas_create_release.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/generate_or_validate_json_schemas.py` & `bo4e-202401.1.0rc2/generate_or_validate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tox.ini` & `bo4e-202401.1.0rc2/tox.ini`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/.github/dependabot.yml` & `bo4e-202401.1.0rc2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md` & `bo4e-202401.1.0rc2/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md` & `bo4e-202401.1.0rc2/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/.github/workflows/codeql-analysis.yml` & `bo4e-202401.1.0rc2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/.github/workflows/coverage.yml` & `bo4e-202401.1.0rc2/.github/workflows/coverage.yml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 on: [push,pull_request]
 jobs:
   coverage:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.12"]
         os: [ubuntu-latest]
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `bo4e-202401.1.0rc1/.github/workflows/dependabot_automerge.yml` & `bo4e-202401.1.0rc2/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/.github/workflows/linting.yml` & `bo4e-202401.1.0rc2/.github/workflows/linting.yml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 on: [push,pull_request]
 jobs:
   linting:
     name: Python Code Quality and Lint
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.12"]
         os: [ubuntu-latest, windows-latest]
         linter-env: ["linting", "type_check", "dev"]
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
```

### Comparing `bo4e-202401.1.0rc1/.github/workflows/packaging_test.yml` & `bo4e-202401.1.0rc2/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/.github/workflows/python-publish-scheduled.yml` & `bo4e-202401.1.0rc2/.github/workflows/python-publish-scheduled.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/.github/workflows/python-publish.yml` & `bo4e-202401.1.0rc2/.github/workflows/python-publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 jobs:
   tests:
     if: startsWith(github.ref, 'refs/tags/v')
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.12"]
         os: [ubuntu-latest]
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `bo4e-202401.1.0rc1/.github/workflows/tests.yml` & `bo4e-202401.1.0rc2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/dev_requirements/requirements-packaging.txt` & `bo4e-202401.1.0rc2/dev_requirements/requirements-packaging.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,80 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.12
+# by the following command:
 #
-#    pip-compile requirements-packaging.in
+#    pip-compile '.\dev_requirements\requirements-packaging.in'
 #
-build==1.0.3
+build==1.2.1
     # via -r requirements-packaging.in
-certifi==2023.7.22
+certifi==2024.2.2
     # via requests
 cffi==1.16.0
     # via cryptography
-charset-normalizer==3.2.0
+charset-normalizer==3.3.2
     # via requests
-cryptography==42.0.2
+cryptography==42.0.5
     # via secretstorage
 docutils==0.20.1
     # via readme-renderer
-idna==3.4
+idna==3.7
     # via requests
-importlib-metadata==6.8.0
+importlib-metadata==7.1.0
     # via
     #   keyring
     #   twine
-jaraco-classes==3.3.0
+jaraco-classes==3.4.0
+    # via keyring
+jaraco-context==5.0.0
+    # via keyring
+jaraco-functools==4.0.0
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-keyring==24.2.0
+keyring==25.1.0
     # via twine
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
-more-itertools==10.1.0
-    # via jaraco-classes
-nh3==0.2.14
+more-itertools==10.2.0
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
+nh3==0.2.17
     # via readme-renderer
-packaging==23.1
+packaging==24.0
     # via build
-pkginfo==1.9.6
+pkginfo==1.10.0
     # via twine
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pygments==2.16.1
+pygments==2.17.2
     # via
     #   readme-renderer
     #   rich
 pyproject-hooks==1.0.0
     # via build
-readme-renderer==42.0
+readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.5.3
+rich==13.7.1
     # via twine
 secretstorage==3.3.3
     # via keyring
 twine==5.0.0
     # via -r requirements-packaging.in
-urllib3==2.0.7
+urllib3==2.2.1
     # via
     #   requests
     #   twine
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
```

### Comparing `bo4e-202401.1.0rc1/dev_requirements/requirements-type_check.txt` & `bo4e-202401.1.0rc2/dev_requirements/requirements-type_check.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile '.\requirements-type_check.in'
 #
-exceptiongroup==1.2.0
-    # via pytest
 iniconfig==2.0.0
     # via pytest
-mypy==1.8.0
+mypy==1.9.0
     # via -r requirements-type_check.in
 mypy-extensions==1.0.0
     # via mypy
 networkx==3.2
     # via networkx-stubs
 networkx-stubs==0.0.1
     # via -r requirements-type_check.in
 packaging==23.1
     # via pytest
-pluggy==1.3.0
+pluggy==1.4.0
     # via pytest
-pytest==8.0.0
+pytest==8.1.1
     # via -r requirements-type_check.in
-tomli==2.0.1
-    # via
-    #   mypy
-    #   pytest
-types-requests==2.31.0.20240125
+types-requests==2.31.0.20240406
     # via -r requirements-type_check.in
 typing-extensions==4.8.0
     # via mypy
 urllib3==2.0.7
     # via types-requests
```

### Comparing `bo4e-202401.1.0rc1/docs/Makefile` & `bo4e-202401.1.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/docs/conf.py` & `bo4e-202401.1.0rc2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 from pathlib import Path
 
 sys.path.insert(0, os.path.join(__location__, "../src"))
 sys.path.insert(0, os.path.join(__location__, "../docs"))
-from uml import PlantUMLNetwork, build_network, compile_files_kroki, write_class_umls
+import uml
 
 # import package bo4e to clarify namespaces and prevent circular import errors
 from bo4e import *
 
 # -- Run sphinx-apidoc ------------------------------------------------------
 # This hack is necessary since RTD does not issue `sphinx-apidoc` before running
 # `sphinx-build -b html . _build/html`. See Issue:
@@ -172,24 +172,19 @@
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-try:
-    from bo4e import __gh_version__ as version
-
-    print(f"Got version {version} from __gh_version__")
-except ImportError:
-    pass
-else:
-    release = version
+from bo4e import __gh_version__ as release
+from bo4e import __version__ as version
 
-print(f"Using version {release} for documentation")
+print(f"Got version = {version} from __version__")
+print(f"Got release = {release} from __gh_version__")
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 # html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 html_logo = "./_static/bo4e-python-logo.png"
@@ -310,15 +305,16 @@
 intersphinx_mapping = {
     "sphinx": ("http://www.sphinx-doc.org/en/stable", None),
     "python": ("https://docs.python.org/" + python_version, None),
 }
 
 # Create UML diagrams in plantuml format. Compile these into svg files into the _static folder.
 # See docs/uml.py for more details.
+uml.LINK_URI_BASE = f"https://bo4e-python.readthedocs.io/en/{release}"
 _exec_plantuml = Path(__location__) / "plantuml.jar"
-_network, _namespaces_to_parse = build_network(Path(module_dir), PlantUMLNetwork)
+_network, _namespaces_to_parse = uml.build_network(Path(module_dir), uml.PlantUMLNetwork)
 print(_network)
-write_class_umls(_network, _namespaces_to_parse, Path(output_dir) / "uml")
+uml.write_class_umls(_network, _namespaces_to_parse, Path(output_dir) / "uml")
 print("Created uml files.")
 
-compile_files_kroki(Path(output_dir) / "uml", Path(output_dir).parent / "_static" / "images")
+uml.compile_files_kroki(Path(output_dir) / "uml", Path(output_dir).parent / "_static" / "images")
 print(f"Compiled uml files into svg using kroki.")
```

### Comparing `bo4e-202401.1.0rc1/docs/index.rst` & `bo4e-202401.1.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/docs/release_workflow.rst` & `bo4e-202401.1.0rc2/docs/release_workflow.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/docs/requirements.txt` & `bo4e-202401.1.0rc2/docs/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # via requests
 charset-normalizer==2.1.0
     # via requests
 docutils==0.18.1
     # via
     #   sphinx
     #   sphinx-rtd-theme
-idna==3.3
+idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
 iso3166==2.1.1
     # via -r requirements.in
 jinja2==3.1.3
     # via sphinx
```

### Comparing `bo4e-202401.1.0rc1/docs/uml.py` & `bo4e-202401.1.0rc2/docs/uml.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/docs/versioning.rst` & `bo4e-202401.1.0rc2/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/docs/_static/bo4e-python-favicon.png` & `bo4e-202401.1.0rc2/docs/_static/bo4e-python-favicon.png`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/docs/_static/bo4e-python-favicon.svg` & `bo4e-202401.1.0rc2/docs/_static/bo4e-python-favicon.svg`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/docs/_static/bo4e-python-logo.png` & `bo4e-202401.1.0rc2/docs/_static/bo4e-python-logo.png`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/docs/_static/bo4e-python-logo.svg` & `bo4e-202401.1.0rc2/docs/_static/bo4e-python-logo.svg`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/docs/_static/bo4e-release-workflow.excalidraw` & `bo4e-202401.1.0rc2/docs/_static/bo4e-release-workflow.excalidraw`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/docs/_static/bo4e-release-workflow.png` & `bo4e-202401.1.0rc2/docs/_static/bo4e-release-workflow.png`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/__init__.py` & `bo4e-202401.1.0rc2/src/bo4e/__init__.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/version.py` & `bo4e-202401.1.0rc2/src/bo4e/version.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/zusatzattribut.py` & `bo4e-202401.1.0rc2/src/bo4e/zusatzattribut.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/angebot.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/angebot.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/ausschreibung.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/ausschreibung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/buendelvertrag.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/energiemenge.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/energiemenge.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/fremdkosten.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/geraet.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/geschaeftsobjekt.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/geschaeftsobjekt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/geschaeftspartner.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/geschaeftspartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/kosten.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/kosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/lastgang.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/lastgang.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/marktlokation.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/marktlokation.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from pydantic import Field
 
 from ..com.adresse import Adresse
 from ..com.geokoordinaten import Geokoordinaten
 from ..com.katasteradresse import Katasteradresse
 from ..com.messlokationszuordnung import Messlokationszuordnung
+from ..com.verbrauch import Verbrauch
+from ..com.zaehlwerk import Zaehlwerk
 from ..enum.bilanzierungsmethode import Bilanzierungsmethode
 from ..enum.energierichtung import Energierichtung
 from ..enum.gasqualitaet import Gasqualitaet
 from ..enum.gebiettyp import Gebiettyp
 from ..enum.kundentyp import Kundentyp
 from ..enum.netzebene import Netzebene
 from ..enum.sparte import Sparte
@@ -111,7 +113,15 @@
     """
     Alternativ zu einer postalischen Adresse und Geokoordinaten kann hier eine Ortsangabe mittels Gemarkung und
     Flurstück erfolgen.
     """
 
     kundengruppen: Optional[list[Kundentyp]] = None
     #: Kundengruppen der Marktlokation
+
+    regelzone: Optional[
+        str
+    ] = None  #: für Strom. Code vom EIC, https://www.entsoe.eu/data/energy-identification-codes-eic/eic-approved-codes/
+    marktgebiet: Optional[str] = None  #: für Gas. Code vom EIC, https://www.entsog.eu/data/data-portal/codes-list
+    zaehlwerke: Optional[list[Zaehlwerk]] = None
+    verbrauchsmengen: Optional[list[Verbrauch]] = None
+    zaehlwerke_der_beteiligten_marktrolle: Optional[list[Zaehlwerk]] = None
```

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/marktteilnehmer.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/marktteilnehmer.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/messlokation.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/messlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/person.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/person.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/preisblatt.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/preisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/preisblattdienstleistung.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/preisblattdienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/preisblatthardware.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/preisblatthardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/preisblattkonzessionsabgabe.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/preisblattkonzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/preisblattmessung.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/preisblattmessung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/preisblattnetznutzung.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/rechnung.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/region.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/region.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/regionaltarif.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/regionaltarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/standorteigenschaften.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/standorteigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/tarif.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/tarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/tarifinfo.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/tarifinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/tarifkosten.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/tarifpreisblatt.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/tarifpreisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/vertrag.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/vertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/zaehler.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/zaehler.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/bo/zeitreihe.py` & `bo4e-202401.1.0rc2/src/bo4e/bo/zeitreihe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/adresse.py` & `bo4e-202401.1.0rc2/src/bo4e/com/adresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/angebotsposition.py` & `bo4e-202401.1.0rc2/src/bo4e/com/angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/angebotsteil.py` & `bo4e-202401.1.0rc2/src/bo4e/com/angebotsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/angebotsvariante.py` & `bo4e-202401.1.0rc2/src/bo4e/com/angebotsvariante.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/aufabschlag.py` & `bo4e-202401.1.0rc2/src/bo4e/com/aufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/aufabschlagproort.py` & `bo4e-202401.1.0rc2/src/bo4e/com/aufabschlagproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/aufabschlagregional.py` & `bo4e-202401.1.0rc2/src/bo4e/com/aufabschlagregional.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/aufabschlagstaffelproort.py` & `bo4e-202401.1.0rc2/src/bo4e/com/aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/ausschreibungsdetail.py` & `bo4e-202401.1.0rc2/src/bo4e/com/ausschreibungsdetail.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/ausschreibungslos.py` & `bo4e-202401.1.0rc2/src/bo4e/com/ausschreibungslos.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/betrag.py` & `bo4e-202401.1.0rc2/src/bo4e/com/betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/com.py` & `bo4e-202401.1.0rc2/src/bo4e/com/com.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/dienstleistung.py` & `bo4e-202401.1.0rc2/src/bo4e/com/dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/energieherkunft.py` & `bo4e-202401.1.0rc2/src/bo4e/com/energieherkunft.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/energiemix.py` & `bo4e-202401.1.0rc2/src/bo4e/com/energiemix.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/fremdkostenblock.py` & `bo4e-202401.1.0rc2/src/bo4e/com/fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/fremdkostenposition.py` & `bo4e-202401.1.0rc2/src/bo4e/com/fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/geokoordinaten.py` & `bo4e-202401.1.0rc2/src/bo4e/com/geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/katasteradresse.py` & `bo4e-202401.1.0rc2/src/bo4e/com/katasteradresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/kontaktweg.py` & `bo4e-202401.1.0rc2/src/bo4e/com/kontaktweg.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/konzessionsabgabe.py` & `bo4e-202401.1.0rc2/src/bo4e/com/konzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/kostenblock.py` & `bo4e-202401.1.0rc2/src/bo4e/com/kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/kostenposition.py` & `bo4e-202401.1.0rc2/src/bo4e/com/kostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/kriteriumwert.py` & `bo4e-202401.1.0rc2/src/bo4e/com/kriteriumwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/marktgebietinfo.py` & `bo4e-202401.1.0rc2/src/bo4e/com/marktgebietinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/menge.py` & `bo4e-202401.1.0rc2/src/bo4e/com/menge.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/messlokationszuordnung.py` & `bo4e-202401.1.0rc2/src/bo4e/com/messlokationszuordnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/positionsaufabschlag.py` & `bo4e-202401.1.0rc2/src/bo4e/com/positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/preis.py` & `bo4e-202401.1.0rc2/src/bo4e/com/preis.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/preisgarantie.py` & `bo4e-202401.1.0rc2/src/bo4e/com/preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/preisposition.py` & `bo4e-202401.1.0rc2/src/bo4e/com/preisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/preisstaffel.py` & `bo4e-202401.1.0rc2/src/bo4e/com/preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/rechnungsposition.py` & `bo4e-202401.1.0rc2/src/bo4e/com/rechnungsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/regionalegueltigkeit.py` & `bo4e-202401.1.0rc2/src/bo4e/com/regionalegueltigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/regionalepreisgarantie.py` & `bo4e-202401.1.0rc2/src/bo4e/com/regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/regionalepreisstaffel.py` & `bo4e-202401.1.0rc2/src/bo4e/com/regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/regionaleraufabschlag.py` & `bo4e-202401.1.0rc2/src/bo4e/com/regionaleraufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/regionaletarifpreisposition.py` & `bo4e-202401.1.0rc2/src/bo4e/com/regionaletarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/regionskriterium.py` & `bo4e-202401.1.0rc2/src/bo4e/com/regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/sigmoidparameter.py` & `bo4e-202401.1.0rc2/src/bo4e/com/sigmoidparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/standorteigenschaftengas.py` & `bo4e-202401.1.0rc2/src/bo4e/com/standorteigenschaftengas.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/standorteigenschaftenstrom.py` & `bo4e-202401.1.0rc2/src/bo4e/com/standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/steuerbetrag.py` & `bo4e-202401.1.0rc2/src/bo4e/com/steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/tarifberechnungsparameter.py` & `bo4e-202401.1.0rc2/src/bo4e/com/tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/tarifeinschraenkung.py` & `bo4e-202401.1.0rc2/src/bo4e/com/tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/tarifpreis.py` & `bo4e-202401.1.0rc2/src/bo4e/com/tarifpreis.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/tarifpreisposition.py` & `bo4e-202401.1.0rc2/src/bo4e/com/tarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/tarifpreispositionproort.py` & `bo4e-202401.1.0rc2/src/bo4e/com/tarifpreispositionproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/tarifpreisstaffelproort.py` & `bo4e-202401.1.0rc2/src/bo4e/com/tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/unterschrift.py` & `bo4e-202401.1.0rc2/src/bo4e/com/unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/verbrauch.py` & `bo4e-202401.1.0rc2/src/bo4e/com/verbrauch.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/vertragskonditionen.py` & `bo4e-202401.1.0rc2/src/bo4e/com/vertragskonditionen.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/vertragsteil.py` & `bo4e-202401.1.0rc2/src/bo4e/com/vertragsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/verwendungszweckpromarktrolle.py` & `bo4e-202401.1.0rc2/src/bo4e/com/verwendungszweckpromarktrolle.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/zaehlwerk.py` & `bo4e-202401.1.0rc2/src/bo4e/com/zaehlwerk.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/zaehlzeitregister.py` & `bo4e-202401.1.0rc2/src/bo4e/com/zaehlzeitregister.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/zeitraum.py` & `bo4e-202401.1.0rc2/src/bo4e/com/zeitraum.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/zeitreihenwert.py` & `bo4e-202401.1.0rc2/src/bo4e/com/zeitreihenwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/zeitspanne.py` & `bo4e-202401.1.0rc2/src/bo4e/com/zeitspanne.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/com/zustaendigkeit.py` & `bo4e-202401.1.0rc2/src/bo4e/com/zustaendigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/abgabeart.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/abgabeart.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/angebotsstatus.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/angebotsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/artikelid.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/artikelid.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/aufabschlagsziel.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/aufabschlagsziel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/ausschreibungsportal.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/ausschreibungsportal.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/bdewartikelnummer.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/bdewartikelnummer.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/bemessungsgroesse.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/bemessungsgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/bilanzierungsmethode.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/bilanzierungsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/dienstleistungstyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/dienstleistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/erzeugungsart.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/erzeugungsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/gebiettyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/gebiettyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/geraeteklasse.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/geraeteklasse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/geraetetyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/geraetetyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/gueltigkeitstyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/gueltigkeitstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/kalkulationsmethode.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/kalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/kostenklasse.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/kostenklasse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/kundengruppe.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/kundengruppe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/kundengruppeka.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/kundengruppeka.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/kundentyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/kundentyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/leistungstyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/leistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/mengeneinheit.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/mengeneinheit.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/messgroesse.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/messgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/messpreistyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/messpreistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/messwertstatus.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/messwertstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/messwertstatuszusatz.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/messwertstatuszusatz.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/netzebene.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/netzebene.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/netznutzungrechnungstyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/netznutzungrechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/oekolabel.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/oekolabel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/oekozertifikat.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/oekozertifikat.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/preisgarantietyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/preisgarantietyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/preistyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/preistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/rechnungslegung.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/rechnungslegung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/rechnungsstatus.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/rechnungsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/rechnungstyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/rechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/regionskriteriumtyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/regionskriteriumtyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/steuerkennzeichen.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/steuerkennzeichen.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/tarifkalkulationsmethode.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/tarifkalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/tarifmerkmal.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/tarifmerkmal.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/themengebiet.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/themengebiet.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/typ.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/typ.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/vertragsart.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/vertragsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/vertragsstatus.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/vertragsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/verwendungszweck.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/verwendungszweck.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/voraussetzungen.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/voraussetzungen.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/waehrungscode.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/waehrungscode.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/zaehlergroesse.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/zaehlergroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/src/bo4e/enum/zaehlertyp.py` & `bo4e-202401.1.0rc2/src/bo4e/enum/zaehlertyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/serialization_helper.py` & `bo4e-202401.1.0rc2/tests/serialization_helper.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_adresse.py` & `bo4e-202401.1.0rc2/tests/test_adresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_angebot.py` & `bo4e-202401.1.0rc2/tests/test_angebot.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_angebotsposition.py` & `bo4e-202401.1.0rc2/tests/test_angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_angebotsteil.py` & `bo4e-202401.1.0rc2/tests/test_angebotsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_angebotsvariante.py` & `bo4e-202401.1.0rc2/tests/test_angebotsvariante.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_aufabschlag.py` & `bo4e-202401.1.0rc2/tests/test_aufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_aufabschlagproort.py` & `bo4e-202401.1.0rc2/tests/test_aufabschlagproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_aufabschlagregional.py` & `bo4e-202401.1.0rc2/tests/test_aufabschlagregional.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_aufabschlagstaffelproort.py` & `bo4e-202401.1.0rc2/tests/test_aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_ausschreibung.py` & `bo4e-202401.1.0rc2/tests/test_ausschreibung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_ausschreibungsdetail.py` & `bo4e-202401.1.0rc2/tests/test_ausschreibungsdetail.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_ausschreibungslos.py` & `bo4e-202401.1.0rc2/tests/test_ausschreibungslos.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_betrag.py` & `bo4e-202401.1.0rc2/tests/test_betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_buendelvertrag.py` & `bo4e-202401.1.0rc2/tests/test_buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_energieherkunft.py` & `bo4e-202401.1.0rc2/tests/test_energieherkunft.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_energiemenge.py` & `bo4e-202401.1.0rc2/tests/test_energiemenge.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_energiemix.py` & `bo4e-202401.1.0rc2/tests/test_energiemix.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_enums.py` & `bo4e-202401.1.0rc2/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_fremdkosten.py` & `bo4e-202401.1.0rc2/tests/test_fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_fremdkostenblock.py` & `bo4e-202401.1.0rc2/tests/test_fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_fremdkostenposition.py` & `bo4e-202401.1.0rc2/tests/test_fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_geokoordinaten.py` & `bo4e-202401.1.0rc2/tests/test_geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_geraet.py` & `bo4e-202401.1.0rc2/tests/test_geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_geschaeftsobjekt.py` & `bo4e-202401.1.0rc2/tests/test_geschaeftsobjekt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_geschaeftspartner.py` & `bo4e-202401.1.0rc2/tests/test_geschaeftspartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_katasteradresse.py` & `bo4e-202401.1.0rc2/tests/test_katasteradresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_kontakt.py` & `bo4e-202401.1.0rc2/tests/test_kontakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_kosten.py` & `bo4e-202401.1.0rc2/tests/test_kosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_kostenblock.py` & `bo4e-202401.1.0rc2/tests/test_kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_kostenposition.py` & `bo4e-202401.1.0rc2/tests/test_kostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_kriteriumswert.py` & `bo4e-202401.1.0rc2/tests/test_kriteriumswert.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_lastgang.py` & `bo4e-202401.1.0rc2/tests/test_lastgang.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_marktgebietinfo.py` & `bo4e-202401.1.0rc2/tests/test_marktgebietinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_marktlokation.py` & `bo4e-202401.1.0rc2/tests/test_marktlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_marktteilnehmer.py` & `bo4e-202401.1.0rc2/tests/test_marktteilnehmer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class TestMarktteilnehmer:
     @pytest.mark.parametrize(
         "marktteilnehmer",
         [
             pytest.param(
                 Marktteilnehmer(
-                    marktrolle=Marktrolle.DL,
+                    marktrolle=Marktrolle.DP,
                     rollencodenummer="9903916000000",
                     rollencodetyp=Rollencodetyp.BDEW,
                     sparte=Sparte.STROM,
                     makoadresse=["stringadressewarum", "as4adresse"],
                     geschaeftspartner=Geschaeftspartner(),
                 )
             )
```

### Comparing `bo4e-202401.1.0rc1/tests/test_menge.py` & `bo4e-202401.1.0rc2/tests/test_menge.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_messlokation.py` & `bo4e-202401.1.0rc2/tests/test_messlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_messlokationszuordnung.py` & `bo4e-202401.1.0rc2/tests/test_messlokationszuordnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_person.py` & `bo4e-202401.1.0rc2/tests/test_person.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_positionsaufabschlag.py` & `bo4e-202401.1.0rc2/tests/test_positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_preis.py` & `bo4e-202401.1.0rc2/tests/test_preis.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_preisblatt.py` & `bo4e-202401.1.0rc2/tests/test_preisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_preisblatt_dienstleistung.py` & `bo4e-202401.1.0rc2/tests/test_preisblatt_dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_preisblatt_hardware.py` & `bo4e-202401.1.0rc2/tests/test_preisblatt_hardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_preisblatt_konzessionsabgabe.py` & `bo4e-202401.1.0rc2/tests/test_preisblatt_konzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_preisblatt_messung.py` & `bo4e-202401.1.0rc2/tests/test_preisblatt_messung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_preisblattnetznutzung.py` & `bo4e-202401.1.0rc2/tests/test_preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_preisgarantie.py` & `bo4e-202401.1.0rc2/tests/test_preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_preisposition.py` & `bo4e-202401.1.0rc2/tests/test_preisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_preisstaffel.py` & `bo4e-202401.1.0rc2/tests/test_preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_rechnung.py` & `bo4e-202401.1.0rc2/tests/test_rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_rechnungsposition.py` & `bo4e-202401.1.0rc2/tests/test_rechnungsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_region.py` & `bo4e-202401.1.0rc2/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_regionalegueltigkeit.py` & `bo4e-202401.1.0rc2/tests/test_regionalegueltigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_regionalepreisgarantie.py` & `bo4e-202401.1.0rc2/tests/test_regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_regionalepreisstaffel.py` & `bo4e-202401.1.0rc2/tests/test_regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_regionaleraufabschlag.py` & `bo4e-202401.1.0rc2/tests/test_regionaleraufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_regionaletarifpreisposition.py` & `bo4e-202401.1.0rc2/tests/test_regionaletarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_regionaltarif.py` & `bo4e-202401.1.0rc2/tests/test_regionaltarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_regionskriterium.py` & `bo4e-202401.1.0rc2/tests/test_regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_sigmoidparameter.py` & `bo4e-202401.1.0rc2/tests/test_sigmoidparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_standorteigenschaften.py` & `bo4e-202401.1.0rc2/tests/test_standorteigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_standorteigenschaftengas.py` & `bo4e-202401.1.0rc2/tests/test_standorteigenschaftengas.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_standorteigenschaftenstrom.py` & `bo4e-202401.1.0rc2/tests/test_standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_steuerbetrag.py` & `bo4e-202401.1.0rc2/tests/test_steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_tarif.py` & `bo4e-202401.1.0rc2/tests/test_tarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_tarifberechnungsparameter.py` & `bo4e-202401.1.0rc2/tests/test_tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_tarifeinschraenkung.py` & `bo4e-202401.1.0rc2/tests/test_tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_tarifinfo.py` & `bo4e-202401.1.0rc2/tests/test_tarifinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_tarifkosten.py` & `bo4e-202401.1.0rc2/tests/test_tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_tarifpreis.py` & `bo4e-202401.1.0rc2/tests/test_tarifpreis.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_tarifpreisblatt.py` & `bo4e-202401.1.0rc2/tests/test_tarifpreisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_tarifpreisposition.py` & `bo4e-202401.1.0rc2/tests/test_tarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_tarifpreispositionproort.py` & `bo4e-202401.1.0rc2/tests/test_tarifpreispositionproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_tarifpreisstaffelproort.py` & `bo4e-202401.1.0rc2/tests/test_tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_unterschrift.py` & `bo4e-202401.1.0rc2/tests/test_unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_verbrauch.py` & `bo4e-202401.1.0rc2/tests/test_verbrauch.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_vertrag.py` & `bo4e-202401.1.0rc2/tests/test_vertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_vertragskonditionen.py` & `bo4e-202401.1.0rc2/tests/test_vertragskonditionen.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_vertragsteil.py` & `bo4e-202401.1.0rc2/tests/test_vertragsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_zaehler.py` & `bo4e-202401.1.0rc2/tests/test_zaehler.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_zeitraum.py` & `bo4e-202401.1.0rc2/tests/test_zeitraum.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_zeitreihe.py` & `bo4e-202401.1.0rc2/tests/test_zeitreihe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_zeitreihenwert.py` & `bo4e-202401.1.0rc2/tests/test_zeitreihenwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_zeitspanne.py` & `bo4e-202401.1.0rc2/tests/test_zeitspanne.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/test_zusatz_attribut.py` & `bo4e-202401.1.0rc2/tests/test_zusatz_attribut.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/tests/utils.py` & `bo4e-202401.1.0rc2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/.gitignore` & `bo4e-202401.1.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/LICENSE.rst` & `bo4e-202401.1.0rc2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.0rc1/pyproject.toml` & `bo4e-202401.1.0rc2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 # This list must be in synq with the ./requirements.in file!
 dependencies = ["iso3166", "pydantic>=2.0.0", "pyhumps"]
 dynamic = ["readme", "version"]
 
 [project.urls]
 Changelog = "https://github.com/bo4e/bo4e-python/releases"
```

### Comparing `bo4e-202401.1.0rc1/PKG-INFO` & `bo4e-202401.1.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: bo4e
-Version: 202401.1.0rc1
+Version: 202401.1.0rc2
 Summary: Python Library that implements the BO4E Standard.
 Project-URL: Changelog, https://github.com/bo4e/bo4e-python/releases
 Project-URL: Homepage, https://github.com/bo4e/bo4e-python
 Project-URL: Documentation, https://bo4e-python.readthedocs.io/en/latest/
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>, Leon Haffmans <leon.haffmans@hochfrequenz.de>, Annika Schlögl <annika.schloegl@hochfrequenz.de>, Franziska Vesely <franziska.vesely@hochfrequenz.de>, Konstantin Klein <konstantin.klein@hochfrequenz.de>
 License: MIT
 License-File: AUTHORS.rst
@@ -14,14 +14,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: iso3166
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: pyhumps
 Description-Content-Type: text/x-rst
 
 =============
```

