# Events

### BeforeInitialization

> threedpc-admin\LaravelFileManager\Events\BeforeInitialization

Example:

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\BeforeInitialization',
    function ($event) {
        
    }
);
```

### DiskSelected

> threedpc-admin\LaravelFileManager\Events\DiskSelected

Example:

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\DiskSelected',
    function ($event) {
        \Log::info('DiskSelected:', [$event->disk()]);
    }
);
```

### FilesUploading

> threedpc-admin\LaravelFileManager\Events\FilesUploading

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\FilesUploading',
    function ($event) {
        \Log::info('FilesUploading:', [
            $event->disk(),
            $event->path(),
            $event->files(),
            $event->overwrite(),
        ]);
    }
);
```

### FilesUploaded

> threedpc-admin\LaravelFileManager\Events\FilesUploaded

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\FilesUploaded',
    function ($event) {
        \Log::info('FilesUploaded:', [
            $event->disk(),
            $event->path(),
            $event->files(),
            $event->overwrite(),
        ]);
    }
);
```

### Deleting

> threedpc-admin\LaravelFileManager\Events\Deleting

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\Deleting',
    function ($event) {
        \Log::info('Deleting:', [
            $event->disk(),
            $event->items(),
        ]);
    }
);
```

### Deleted

> threedpc-admin\LaravelFileManager\Events\Deleted

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\Deleted',
    function ($event) {
        \Log::info('Deleted:', [
            $event->disk(),
            $event->items(),
        ]);
    }
);
```

### Paste

> threedpc-admin\LaravelFileManager\Events\Paste

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\Paste',
    function ($event) {
        \Log::info('Paste:', [
            $event->disk(),
            $event->path(),
            $event->clipboard(),
        ]);
    }
);
```

### Rename

> threedpc-admin\LaravelFileManager\Events\Rename

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\Rename',
    function ($event) {
        \Log::info('Rename:', [
            $event->disk(),
            $event->newName(),
            $event->oldName(),
            $event->type(), // 'file' or 'dir'
        ]);
    }
);
```

### Download

> threedpc-admin\LaravelFileManager\Events\Download

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\Download',
    function ($event) {
        \Log::info('Download:', [
            $event->disk(),
            $event->path(),
        ]);
    }
);
```

*When using a text editor, the file you are editing is also downloaded! And this event is triggered!*

### DirectoryCreating

> threedpc-admin\LaravelFileManager\Events\DirectoryCreating

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\DirectoryCreating',
    function ($event) {
        \Log::info('DirectoryCreating:', [
            $event->disk(),
            $event->path(),
            $event->name(),
        ]);
    }
);
```

### DirectoryCreated

> threedpc-admin\LaravelFileManager\Events\DirectoryCreated

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\DirectoryCreated',
    function ($event) {
        \Log::info('DirectoryCreated:', [
            $event->disk(),
            $event->path(),
            $event->name(),
        ]);
    }
);
```

### FileCreating

> threedpc-admin\LaravelFileManager\Events\FileCreating

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\FileCreating',
    function ($event) {
        \Log::info('FileCreating:', [
            $event->disk(),
            $event->path(),
            $event->name(),
        ]);
    }
);
```

### FileCreated

> threedpc-admin\LaravelFileManager\Events\FileCreated

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\FileCreated',
    function ($event) {
        \Log::info('FileCreated:', [
            $event->disk(),
            $event->path(),
            $event->name(),
        ]);
    }
);
```

### FileUpdate

> threedpc-admin\LaravelFileManager\Events\FileUpdate

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\FileUpdate',
    function ($event) {
        \Log::info('FileUpdate:', [
            $event->disk(),
            $event->path(),
        ]);
    }
);
```

### Zip

> threedpc-admin\LaravelFileManager\Events\Zip

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\Zip',
    function ($event) {
        \Log::info('Zip:', [
            $event->disk(),
            $event->path(),
            $event->name(),
            $event->elements(),
        ]);
    }
);
```

### ZipCreated

> threedpc-admin\LaravelFileManager\Events\ZipCreated

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\ZipCreated',
    function ($event) {
        \Log::info('ZipCreated:', [
            $event->disk(),
            $event->path(),
            $event->name(),
            $event->elements(),
        ]);
    }
);
```

### ZipFailed

> threedpc-admin\LaravelFileManager\Events\ZipCreated

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\ZipFailed',
    function ($event) {
        \Log::info('ZipFailed:', [
            $event->disk(),
            $event->path(),
            $event->name(),
            $event->elements(),
        ]);
    }
);
```

### Unzip

> threedpc-admin\LaravelFileManager\Events\Unzip

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\Unzip',
    function ($event) {
        \Log::info('Unzip:', [
            $event->disk(),
            $event->path(),
            $event->folder(),
        ]);
    }
);
```

### UnzipCreated

> threedpc-admin\LaravelFileManager\Events\UnzipCreated

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\UnzipCreated',
    function ($event) {
        \Log::info('UnzipCreated:', [
            $event->disk(),
            $event->path(),
            $event->folder(),
        ]);
    }
);
```

### UnzipFailed

> threedpc-admin\LaravelFileManager\Events\UnzipFailed

```php
\Event::listen('threedpc-admin\LaravelFileManager\Events\UnzipFailed',
    function ($event) {
        \Log::info('UnzipFailed:', [
            $event->disk(),
            $event->path(),
            $event->folder(),
        ]);
    }
);
```
