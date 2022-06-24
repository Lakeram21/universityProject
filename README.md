
# Scafold a new controller with views
dotnet-aspnet-codegenerator controller -name StudentsController -m Student -dc SchoolContext --relativeFolderPath Controllers --useDefaultLayout --referenceScriptLibraries -sqlite



# Migrations
dotnet ef database drop
dotnet ef migrations add InitialCreate
dotnet ef database update