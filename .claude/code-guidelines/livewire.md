# Livewire guidelines

## Component Structure

- Use a single responsibility approach for Livewire components.
- Use PascalCase for component class names (e.g., `NotificationsMenu`).
- Use kebab-case for component view names (e.g., `notifications-menu.blade.php`).
- Place component views in the `resources/views/livewire`.

## Component Implementation

- Use proper type hints and PHPDoc annotations for properties and methods.
- Use the `mount()` method for component initialization.
- Use computed properties for derived data.
- Use actions for handling user interactions.
- Use proper error handling and feedback.
- Use Annotations.
- Use public properties for data binding
- Use lifecycle hooks appropriately (mount, render, updated, etc.)
- Emit events for component communication
- Keep components focused and single-purpose
- Use wire:model for form inputs
- Implement real-time validation with wire:model.lazy or wire:model.debounce
