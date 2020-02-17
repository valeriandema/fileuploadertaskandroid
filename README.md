# fileuploadertaskandroid

Kotlin is chosen because client's requirements

Libraries that are used in the project:
1. Dagger2 - dependency injection

2. Retrofit2 - Rest Client
2.1 Gson - serialisation network response
2.2 OkHttpClient - make HTTPS queries

3. Coroutines - kotlin's extension for handling threads
4. Lifecycle viewmodel - viewmodel that is able to outlive screen rotation in case it should be needed
5. Material - all layouts and widgets are from material design library with cornerFamily - cut

What this app does:
it allows to pick up images from storage (10 at once) and to upload them to server.
Before uploading pictures they are compressed a little
Each image sends in separate thread that can be restarted in case it fails or cancelled
