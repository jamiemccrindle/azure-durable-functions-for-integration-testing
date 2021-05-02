FROM mcr.microsoft.com/azure-functions/dotnet:3.0-dotnet3-core-tools

# RUN export DEBIAN_FRONTEND=noninteractive \
#     && echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $(lsb_release -cs) main" > /etc/apt/sources.list.d/azure-cli.list \
#     && curl -sL https://packages.microsoft.com/keys/microsoft.asc | (OUT=$(apt-key add - 2>&1) || echo $OUT) \
#     && apt-get update \
#     && apt-get install -y azure-cli

RUN curl -Lo /usr/local/bin/bicep https://github.com/Azure/bicep/releases/latest/download/bicep-linux-x64 \
    && chmod +x /usr/local/bin/bicep
