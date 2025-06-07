# BarbezDotEu.Extensions.Caching.Compressed
Compressed encapsulated memory cache based on BarbezDotEu.Extensions.Caching and MessagePack.

## Overview
This library provides a compressed memory caching implementation that uses MessagePack serialization for efficient storage. It extends the functionality of BarbezDotEu.Extensions.Caching by adding compression capabilities.

## Features
- Implements `IEncapsulatedMemoryCache` interface
- Uses MessagePack serialization with LZ4 block array compression
- Built for .NET Standard 2.0
- MIT Licensed

## Dependencies
- BarbezDotEu.Extensions.Caching (>= 3.0.1)
- MessagePack (>= 3.1.3)

## Installation
Install via NuGet:

## Usage
The `CompressedMemoryCache` class provides a memory cache implementation that automatically compresses cached objects using MessagePack serialization.

## CompressedMemoryCache Class
The `CompressedMemoryCache` class implements `IEncapsulatedMemoryCache` and provides compressed object caching using MessagePack serialization with LZ4 block array compression.

### Constructor
- `memoryCache`: An instance of `IMemoryCache` that will be used for the underlying storage.

### Methods

#### Set<TCachable, TCaller>

Retrieves and decompresses an object from the cache:
- `method`: The method name associated with the cache entry
- `differentiator`: The differentiator used when the object was cached
- Returns: The cached object of type `TReturn`, or `null` if not found

## License
Copyright © 2025 Hannes Barbez. All rights reserved.  
Licensed under the MIT License.

## Links
- [Project Website](https://barbez.eu)
- [GitHub Repository](https://github.com/hannesbarbez/BarbezDotEu.Extensions.Caching.Compressed)
