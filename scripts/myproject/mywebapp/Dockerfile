FROM microsoft/dotnet:2.1-aspnetcore-runtime AS base

FROM microsoft/dotnet:2.1-sdk AS build

WORKDIR /mywebapp
COPY bin/release/netcoreapp2.1/publish .

ENV ASPNETCORE_URLS http://+:5000
EXPOSE 5000

ENTRYPOINT ["dotnet", "mywebapp.dll"]