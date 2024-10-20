## API Report File for "@backstage/plugin-catalog"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
/// <reference types="react" />

import { AnyApiFactory } from '@backstage/frontend-plugin-api';
import { AnyExtensionDataRef } from '@backstage/frontend-plugin-api';
import { AnyExtensionInputMap } from '@backstage/frontend-plugin-api';
import { AnyRouteRefParams } from '@backstage/frontend-plugin-api';
import { BackstagePlugin } from '@backstage/frontend-plugin-api';
import { ConfigurableExtensionDataRef } from '@backstage/frontend-plugin-api';
import { Entity } from '@backstage/catalog-model';
import { ExtensionBlueprint } from '@backstage/frontend-plugin-api';
import { ExtensionDefinition } from '@backstage/frontend-plugin-api';
import { ExtensionInput } from '@backstage/frontend-plugin-api';
import { ExternalRouteRef } from '@backstage/frontend-plugin-api';
import { IconComponent } from '@backstage/core-plugin-api';
import { JSX as JSX_2 } from 'react';
import { PortableSchema } from '@backstage/frontend-plugin-api';
import { default as React_2 } from 'react';
import { RouteRef } from '@backstage/frontend-plugin-api';
import { SearchResultItemExtensionComponent } from '@backstage/plugin-search-react/alpha';
import { SearchResultItemExtensionPredicate } from '@backstage/plugin-search-react/alpha';
import { TranslationRef } from '@backstage/core-plugin-api/alpha';

// @alpha
export const CatalogFilterBlueprint: ExtensionBlueprint<
  {
    kind: 'catalog-filter';
    namespace: undefined;
    name: undefined;
  },
  {
    loader: () => Promise<JSX.Element>;
  },
  ConfigurableExtensionDataRef<React_2.JSX.Element, 'core.reactElement', {}>,
  {},
  {},
  {},
  never
>;

// @alpha (undocumented)
export const catalogTranslationRef: TranslationRef<
  'catalog',
  {
    readonly 'deleteEntity.description': 'This entity is not referenced by any location and is therefore not receiving updates. Click here to delete.';
    readonly 'deleteEntity.cancelButtonTitle': 'Cancel';
    readonly 'deleteEntity.deleteButtonTitle': 'Delete';
    readonly 'deleteEntity.dialogTitle': 'Are you sure you want to delete this entity?';
    readonly 'indexPage.title': '{{orgName}} Catalog';
    readonly 'indexPage.createButtonTitle': 'Create';
    readonly 'indexPage.supportButtonContent': 'All your software catalog entities';
    readonly 'aboutCard.title': 'About';
    readonly 'aboutCard.refreshButtonTitle': 'Schedule entity refresh';
    readonly 'aboutCard.editButtonTitle': 'Edit Metadata';
    readonly 'aboutCard.createSimilarButtonTitle': 'Create something similar';
    readonly 'aboutCard.refreshScheduledMessage': 'Refresh scheduled';
    readonly 'aboutCard.launchTemplate': 'Launch Template';
    readonly 'aboutCard.viewTechdocs': 'View TechDocs';
    readonly 'aboutCard.viewSource': 'View Source';
    readonly 'aboutCard.descriptionField.value': 'No description';
    readonly 'aboutCard.descriptionField.label': 'Description';
    readonly 'aboutCard.ownerField.value': 'No Owner';
    readonly 'aboutCard.ownerField.label': 'Owner';
    readonly 'aboutCard.domainField.value': 'No Domain';
    readonly 'aboutCard.domainField.label': 'Domain';
    readonly 'aboutCard.systemField.value': 'No System';
    readonly 'aboutCard.systemField.label': 'System';
    readonly 'aboutCard.parentComponentField.value': 'No Parent Component';
    readonly 'aboutCard.parentComponentField.label': 'Parent Component';
    readonly 'aboutCard.typeField.label': 'Type';
    readonly 'aboutCard.lifecycleField.label': 'Lifecycle';
    readonly 'aboutCard.tagsField.value': 'No Tags';
    readonly 'aboutCard.tagsField.label': 'Tags';
    readonly 'aboutCard.targetsField.label': 'Targets';
    readonly 'searchResultItem.lifecycle': 'Lifecycle';
    readonly 'searchResultItem.Owner': 'Owner';
    readonly 'catalogTable.warningPanelTitle': 'Could not fetch catalog entities.';
    readonly 'catalogTable.viewActionTitle': 'View';
    readonly 'catalogTable.editActionTitle': 'Edit';
    readonly 'catalogTable.starActionTitle': 'Add to favorites';
    readonly 'catalogTable.unStarActionTitle': 'Remove from favorites';
    readonly 'dependencyOfComponentsCard.title': 'Dependency of components';
    readonly 'dependencyOfComponentsCard.emptyMessage': 'No component depends on this component';
    readonly 'dependsOnComponentsCard.title': 'Depends on components';
    readonly 'dependsOnComponentsCard.emptyMessage': 'No component is a dependency of this component';
    readonly 'dependsOnResourcesCard.title': 'Depends on resources';
    readonly 'dependsOnResourcesCard.emptyMessage': 'No resource is a dependency of this component';
    readonly 'entityContextMenu.copiedMessage': 'Copied!';
    readonly 'entityContextMenu.moreButtonTitle': 'More';
    readonly 'entityContextMenu.inspectMenuTitle': 'Inspect entity';
    readonly 'entityContextMenu.copyURLMenuTitle': 'Copy entity URL';
    readonly 'entityContextMenu.unregisterMenuTitle': 'Unregister entity';
    readonly 'entityLabelsCard.title': 'Labels';
    readonly 'entityLabelsCard.emptyDescription': 'No labels defined for this entity. You can add labels to your entity YAML as shown in the highlighted example below:';
    readonly 'entityLabelsCard.readMoreButtonTitle': 'Read more';
    readonly 'entityLabels.warningPanelTitle': 'Entity not found';
    readonly 'entityLabels.ownerLabel': 'Owner';
    readonly 'entityLabels.lifecycleLabel': 'Lifecycle';
    readonly 'entityLinksCard.title': 'Links';
    readonly 'entityLinksCard.emptyDescription': 'No links defined for this entity. You can add links to your entity YAML as shown in the highlighted example below:';
    readonly 'entityLinksCard.readMoreButtonTitle': 'Read more';
    readonly 'entityNotFound.title': 'Entity was not found';
    readonly 'entityNotFound.description': 'Want to help us build this? Check out our Getting Started documentation.';
    readonly 'entityNotFound.docButtonTitle': 'DOCS';
    readonly entityProcessingErrorsDescription: 'The error below originates from';
    readonly entityRelationWarningDescription: "This entity has relations to other entities, which can't be found in the catalog.\n Entities not found are: ";
    readonly 'hasComponentsCard.title': 'Has components';
    readonly 'hasComponentsCard.emptyMessage': 'No component is part of this system';
    readonly 'hasResourcesCard.title': 'Has resources';
    readonly 'hasResourcesCard.emptyMessage': 'No resource is part of this system';
    readonly 'hasSubcomponentsCard.title': 'Has subcomponents';
    readonly 'hasSubcomponentsCard.emptyMessage': 'No subcomponent is part of this component';
    readonly 'hasSubdomainsCard.title': 'Has subdomains';
    readonly 'hasSubdomainsCard.emptyMessage': 'No subdomain is part of this domain';
    readonly 'hasSystemsCard.title': 'Has systems';
    readonly 'hasSystemsCard.emptyMessage': 'No system is part of this domain';
    readonly 'relatedEntitiesCard.emptyHelpLinkTitle': 'Learn how to change this.';
    readonly 'systemDiagramCard.title': 'System Diagram';
    readonly 'systemDiagramCard.description': 'Use pinch & zoo to move around the diagram.';
    readonly 'systemDiagramCard.edgeLabels.dependsOn': 'depends on';
    readonly 'systemDiagramCard.edgeLabels.partOf': 'part of';
    readonly 'systemDiagramCard.edgeLabels.provides': 'provides';
  }
>;

// @alpha @deprecated (undocumented)
export function createCatalogFilterExtension<
  TInputs extends AnyExtensionInputMap,
  TConfig,
>(options: {
  namespace?: string;
  name?: string;
  inputs?: TInputs;
  configSchema?: PortableSchema<TConfig>;
  loader: (options: { config: TConfig }) => Promise<JSX.Element>;
}): ExtensionDefinition<
  TConfig,
  TConfig,
  never,
  never,
  {
    kind?: string | undefined;
    namespace?: string | undefined;
    name?: string | undefined;
  }
>;

// @alpha (undocumented)
const _default: BackstagePlugin<
  {
    catalogIndex: RouteRef<undefined>;
    catalogEntity: RouteRef<{
      name: string;
      kind: string;
      namespace: string;
    }>;
  },
  {
    viewTechDoc: ExternalRouteRef<{
      name: string;
      kind: string;
      namespace: string;
    }>;
    createComponent: ExternalRouteRef<undefined>;
    createFromTemplate: ExternalRouteRef<{
      namespace: string;
      templateName: string;
    }>;
    unregisterRedirect: ExternalRouteRef<undefined>;
  },
  {
    'nav-item:catalog': ExtensionDefinition<
      {},
      {},
      ConfigurableExtensionDataRef<
        {
          title: string;
          icon: IconComponent;
          routeRef: RouteRef<undefined>;
        },
        'core.nav-item.target',
        {}
      >,
      {},
      {
        kind: 'nav-item';
        namespace: undefined;
        name: undefined;
      }
    >;
    'api:catalog/starred-entities': ExtensionDefinition<
      {},
      {},
      ConfigurableExtensionDataRef<AnyApiFactory, 'core.api.factory', {}>,
      {},
      {
        kind: 'api';
        namespace: undefined;
        name: 'starred-entities';
      }
    >;
    'api:catalog/entity-presentation': ExtensionDefinition<
      {},
      {},
      ConfigurableExtensionDataRef<AnyApiFactory, 'core.api.factory', {}>,
      {},
      {
        kind: 'api';
        namespace: undefined;
        name: 'entity-presentation';
      }
    >;
    'entity-card:catalog/about': ExtensionDefinition<
      {
        filter: string | undefined;
      },
      {
        filter?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<
          (entity: Entity) => boolean,
          'catalog.entity-filter-function',
          {
            optional: true;
          }
        >
      | ConfigurableExtensionDataRef<
          string,
          'catalog.entity-filter-expression',
          {
            optional: true;
          }
        >,
      {},
      {
        kind: 'entity-card';
        namespace: undefined;
        name: 'about';
      }
    >;
    'entity-card:catalog/links': ExtensionDefinition<
      {
        filter: string | undefined;
      },
      {
        filter?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<
          (entity: Entity) => boolean,
          'catalog.entity-filter-function',
          {
            optional: true;
          }
        >
      | ConfigurableExtensionDataRef<
          string,
          'catalog.entity-filter-expression',
          {
            optional: true;
          }
        >,
      {},
      {
        kind: 'entity-card';
        namespace: undefined;
        name: 'links';
      }
    >;
    'entity-card:catalog/labels': ExtensionDefinition<
      {
        filter: string | undefined;
      },
      {
        filter?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<
          (entity: Entity) => boolean,
          'catalog.entity-filter-function',
          {
            optional: true;
          }
        >
      | ConfigurableExtensionDataRef<
          string,
          'catalog.entity-filter-expression',
          {
            optional: true;
          }
        >,
      {},
      {
        kind: 'entity-card';
        namespace: undefined;
        name: 'labels';
      }
    >;
    'entity-card:catalog/depends-on-components': ExtensionDefinition<
      {
        filter: string | undefined;
      },
      {
        filter?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<
          (entity: Entity) => boolean,
          'catalog.entity-filter-function',
          {
            optional: true;
          }
        >
      | ConfigurableExtensionDataRef<
          string,
          'catalog.entity-filter-expression',
          {
            optional: true;
          }
        >,
      {},
      {
        kind: 'entity-card';
        namespace: undefined;
        name: 'depends-on-components';
      }
    >;
    'entity-card:catalog/depends-on-resources': ExtensionDefinition<
      {
        filter: string | undefined;
      },
      {
        filter?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<
          (entity: Entity) => boolean,
          'catalog.entity-filter-function',
          {
            optional: true;
          }
        >
      | ConfigurableExtensionDataRef<
          string,
          'catalog.entity-filter-expression',
          {
            optional: true;
          }
        >,
      {},
      {
        kind: 'entity-card';
        namespace: undefined;
        name: 'depends-on-resources';
      }
    >;
    'entity-card:catalog/has-components': ExtensionDefinition<
      {
        filter: string | undefined;
      },
      {
        filter?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<
          (entity: Entity) => boolean,
          'catalog.entity-filter-function',
          {
            optional: true;
          }
        >
      | ConfigurableExtensionDataRef<
          string,
          'catalog.entity-filter-expression',
          {
            optional: true;
          }
        >,
      {},
      {
        kind: 'entity-card';
        namespace: undefined;
        name: 'has-components';
      }
    >;
    'entity-card:catalog/has-resources': ExtensionDefinition<
      {
        filter: string | undefined;
      },
      {
        filter?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<
          (entity: Entity) => boolean,
          'catalog.entity-filter-function',
          {
            optional: true;
          }
        >
      | ConfigurableExtensionDataRef<
          string,
          'catalog.entity-filter-expression',
          {
            optional: true;
          }
        >,
      {},
      {
        kind: 'entity-card';
        namespace: undefined;
        name: 'has-resources';
      }
    >;
    'entity-card:catalog/has-subcomponents': ExtensionDefinition<
      {
        filter: string | undefined;
      },
      {
        filter?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<
          (entity: Entity) => boolean,
          'catalog.entity-filter-function',
          {
            optional: true;
          }
        >
      | ConfigurableExtensionDataRef<
          string,
          'catalog.entity-filter-expression',
          {
            optional: true;
          }
        >,
      {},
      {
        kind: 'entity-card';
        namespace: undefined;
        name: 'has-subcomponents';
      }
    >;
    'entity-card:catalog/has-subdomains': ExtensionDefinition<
      {
        filter: string | undefined;
      },
      {
        filter?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<
          (entity: Entity) => boolean,
          'catalog.entity-filter-function',
          {
            optional: true;
          }
        >
      | ConfigurableExtensionDataRef<
          string,
          'catalog.entity-filter-expression',
          {
            optional: true;
          }
        >,
      {},
      {
        kind: 'entity-card';
        namespace: undefined;
        name: 'has-subdomains';
      }
    >;
    'entity-card:catalog/has-systems': ExtensionDefinition<
      {
        filter: string | undefined;
      },
      {
        filter?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<
          (entity: Entity) => boolean,
          'catalog.entity-filter-function',
          {
            optional: true;
          }
        >
      | ConfigurableExtensionDataRef<
          string,
          'catalog.entity-filter-expression',
          {
            optional: true;
          }
        >,
      {},
      {
        kind: 'entity-card';
        namespace: undefined;
        name: 'has-systems';
      }
    >;
    'entity-content:catalog/overview': ExtensionDefinition<
      {
        [x: string]: any;
      } & {
        path: string | undefined;
        title: string | undefined;
        filter: string | undefined;
      },
      {
        [x: string]: any;
      } & {
        filter?: string | undefined;
        title?: string | undefined;
        path?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<string, 'core.routing.path', {}>
      | ConfigurableExtensionDataRef<
          RouteRef<AnyRouteRefParams>,
          'core.routing.ref',
          {
            optional: true;
          }
        >
      | ConfigurableExtensionDataRef<string, 'catalog.entity-content-title', {}>
      | ConfigurableExtensionDataRef<
          (entity: Entity) => boolean,
          'catalog.entity-filter-function',
          {
            optional: true;
          }
        >
      | ConfigurableExtensionDataRef<
          string,
          'catalog.entity-filter-expression',
          {
            optional: true;
          }
        >,
      {
        cards: ExtensionInput<
          | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
          | ConfigurableExtensionDataRef<
              (entity: Entity) => boolean,
              'catalog.entity-filter-function',
              {
                optional: true;
              }
            >
          | ConfigurableExtensionDataRef<
              string,
              'catalog.entity-filter-expression',
              {
                optional: true;
              }
            >,
          {
            singleton: false;
            optional: false;
          }
        >;
      },
      {
        kind: 'entity-content';
        namespace: undefined;
        name: 'overview';
      }
    >;
    'catalog-filter:catalog/tag': ExtensionDefinition<
      {},
      {},
      ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>,
      {},
      {
        kind: 'catalog-filter';
        namespace: undefined;
        name: 'tag';
      }
    >;
    'catalog-filter:catalog/kind': ExtensionDefinition<
      {
        initialFilter: string;
      },
      {
        initialFilter?: string | undefined;
      },
      ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>,
      {
        [x: string]: ExtensionInput<
          AnyExtensionDataRef,
          {
            optional: boolean;
            singleton: boolean;
          }
        >;
      },
      {
        kind: 'catalog-filter';
        namespace: undefined;
        name: 'kind';
      }
    >;
    'catalog-filter:catalog/type': ExtensionDefinition<
      {},
      {},
      ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>,
      {},
      {
        kind: 'catalog-filter';
        namespace: undefined;
        name: 'type';
      }
    >;
    'catalog-filter:catalog/mode': ExtensionDefinition<
      {
        mode: 'all' | 'owners-only' | undefined;
      },
      {
        mode?: 'all' | 'owners-only' | undefined;
      },
      ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>,
      {
        [x: string]: ExtensionInput<
          AnyExtensionDataRef,
          {
            optional: boolean;
            singleton: boolean;
          }
        >;
      },
      {
        kind: 'catalog-filter';
        namespace: undefined;
        name: 'mode';
      }
    >;
    'catalog-filter:catalog/namespace': ExtensionDefinition<
      {},
      {},
      ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>,
      {},
      {
        kind: 'catalog-filter';
        namespace: undefined;
        name: 'namespace';
      }
    >;
    'catalog-filter:catalog/lifecycle': ExtensionDefinition<
      {},
      {},
      ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>,
      {},
      {
        kind: 'catalog-filter';
        namespace: undefined;
        name: 'lifecycle';
      }
    >;
    'catalog-filter:catalog/processing-status': ExtensionDefinition<
      {},
      {},
      ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>,
      {},
      {
        kind: 'catalog-filter';
        namespace: undefined;
        name: 'processing-status';
      }
    >;
    'catalog-filter:catalog/list': ExtensionDefinition<
      {
        initialFilter: 'all' | 'owned' | 'starred';
      },
      {
        initialFilter?: 'all' | 'owned' | 'starred' | undefined;
      },
      ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>,
      {
        [x: string]: ExtensionInput<
          AnyExtensionDataRef,
          {
            optional: boolean;
            singleton: boolean;
          }
        >;
      },
      {
        kind: 'catalog-filter';
        namespace: undefined;
        name: 'list';
      }
    >;
    'page:catalog': ExtensionDefinition<
      {
        [x: string]: any;
      } & {
        path: string | undefined;
      },
      {
        [x: string]: any;
      } & {
        path?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<string, 'core.routing.path', {}>
      | ConfigurableExtensionDataRef<
          RouteRef<AnyRouteRefParams>,
          'core.routing.ref',
          {
            optional: true;
          }
        >,
      {
        filters: ExtensionInput<
          ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>,
          {
            singleton: false;
            optional: false;
          }
        >;
      },
      {
        kind: 'page';
        namespace: undefined;
        name: undefined;
      }
    >;
    'page:catalog/entity': ExtensionDefinition<
      {
        [x: string]: any;
      } & {
        path: string | undefined;
      },
      {
        [x: string]: any;
      } & {
        path?: string | undefined;
      },
      | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
      | ConfigurableExtensionDataRef<string, 'core.routing.path', {}>
      | ConfigurableExtensionDataRef<
          RouteRef<AnyRouteRefParams>,
          'core.routing.ref',
          {
            optional: true;
          }
        >,
      {
        contents: ExtensionInput<
          | ConfigurableExtensionDataRef<JSX_2.Element, 'core.reactElement', {}>
          | ConfigurableExtensionDataRef<string, 'core.routing.path', {}>
          | ConfigurableExtensionDataRef<
              RouteRef<AnyRouteRefParams>,
              'core.routing.ref',
              {
                optional: true;
              }
            >
          | ConfigurableExtensionDataRef<
              string,
              'catalog.entity-content-title',
              {}
            >
          | ConfigurableExtensionDataRef<
              (entity: Entity) => boolean,
              'catalog.entity-filter-function',
              {
                optional: true;
              }
            >
          | ConfigurableExtensionDataRef<
              string,
              'catalog.entity-filter-expression',
              {
                optional: true;
              }
            >,
          {
            singleton: false;
            optional: false;
          }
        >;
      },
      {
        kind: 'page';
        namespace: undefined;
        name: 'entity';
      }
    >;
    'search-result-list-item:catalog': ExtensionDefinition<
      {
        noTrack: boolean;
      },
      {
        noTrack?: boolean | undefined;
      },
      ConfigurableExtensionDataRef<
        {
          predicate?: SearchResultItemExtensionPredicate | undefined;
          component: SearchResultItemExtensionComponent;
        },
        'search.search-result-list-item.item',
        {}
      >,
      {},
      {
        kind: 'search-result-list-item';
        namespace: undefined;
        name: undefined;
      }
    >;
  }
>;
export default _default;

// (No @packageDocumentation comment for this package)
```
