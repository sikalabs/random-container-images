FROM ghcr.io/sikalabs/ci

# install go
RUN slu s ins go
RUN ln -s /usr/local/go/bin/go /usr/local/bin/go

# install wip slr
COPY --from=ghcr.io/sikalabsregistry/wip/slr /usr/local/bin/slr /usr/local/bin/slr
