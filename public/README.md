# Locorda: Sync offline-first apps using your user's remote storage

> ⚠️ **Pre-Alpha Status**: Locorda is currently under active development. The specification is complete, but the Dart/Flutter implementation is in progress. Not ready for production use.

**Locorda** — the rope that connects and weaves local data together.

## About Locorda

Locorda is a comprehensive specification and Dart/Flutter implementation for building **offline-first applications** that sync seamlessly with **passive storage backends** like Solid Pods, Google Drive, or any file storage system. Users bring their own backend, developers get easy cross-device sync.

### Key Features

- **🔄 Conflict-Free Synchronization**: State-based CRDT algorithms ensure safe collaboration without coordination
- **🌐 Semantic Interoperability**: All data stored as clean, standard RDF for maximum compatibility
- **⚡ Performance at Scale**: Sharded indices handle datasets from 100 to 100,000+ resources
- **📱 Offline-First**: Full offline functionality with sync when connectivity is available
- **🔒 Privacy-Preserving**: User-controlled storage with pluggable access control systems

## Architecture

Locorda follows a **4-layer architecture**:

1. **Data Resource Layer**: Clean RDF resources using standard vocabularies
2. **Merge Contract Layer**: Public CRDT rules for conflict resolution
3. **Indexing Layer**: Efficient change detection and performance optimization
4. **Sync Strategy Layer**: Application-specific performance trade-offs

## Main Repository

**[📦 locorda/locorda](https://github.com/locorda/locorda)** - Complete specification and Dart/Flutter implementation

### Quick Links

- **[📋 Read the Specification](https://github.com/locorda/locorda/blob/main/spec/SPECIFICATION.md)** - Complete technical specification
- **[🌐 RDF Vocabularies & Mappings](https://locorda.dev/)** - Web access to vocabularies and semantic mappings
- **[🚀 Try the Demo](https://locorda.dev/example/personal_notes_app/)** - Live personal notes app demo
- **[💻 Implementation Guide](https://github.com/locorda/locorda/blob/main/IMPLEMENTATION.md)** - Package structure and development workflow

## Project Scope

**Dual Purpose:**
1. **📋 Language-Agnostic Specification** - Complete architectural documentation for implementing CRDT-enabled applications with passive storage backends
2. **🛠️ Dart/Flutter Implementation** - Production-ready multipackage library for building collaborative applications

## Future Local-First

Currently offline-first, Locorda will become truly **local-first** with the addition of end-to-end encryption (planned for v2+). See our [roadmap](https://github.com/locorda/locorda/blob/main/spec/docs/FUTURE-TOPICS.md) for details.

## Standards Alignment

This work aligns with and contributes to:
- **[W3C CRDT for RDF Community Group](https://www.w3.org/community/crdt4rdf/)**
- **[RDF](https://www.w3.org/RDF/)** and **[Linked Data](https://www.w3.org/standards/semanticweb/data)** principles
- **[Solid Protocol](https://solidproject.org/)** ecosystem

## Getting Started

### For Application Developers
```yaml
# Coming soon - not yet published
dependencies:
  locorda: ^0.1.0  # Pre-alpha, in development
```

### For Specification Writers
Start with **[spec/docs/ARCHITECTURE.md](https://github.com/locorda/locorda/blob/main/spec/docs/ARCHITECTURE.md)**

### For Framework Implementers
The specification is **language-agnostic** - implementations in JavaScript, Python, Java, etc. are welcomed!

## Community

- **Issues & Discussions**: [GitHub](https://github.com/locorda/locorda/issues)
- **Specification Discussions**: [W3C CRDT for RDF Community Group](https://www.w3.org/community/crdt4rdf/)**
- **Website**: [locorda.dev](https://locorda.dev)

---

*Bridging the gap between theoretical CRDT research and practical application development with passive storage backends, enabling a new generation of truly collaborative, interoperable applications.*