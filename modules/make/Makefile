## Lint all makefiles
make\:lint:
	@LINT=true \
	 find . -type f -name 'Makefile*' -type f '!' -name '*.example' -exec \
			 /bin/sh -c 'echo "==> {}">/dev/stderr; make --include-dir=modules/ --just-print --dry-run --recon --no-print-directory --quiet --silent -f {}' \; > /dev/null
	@make bash:lint
