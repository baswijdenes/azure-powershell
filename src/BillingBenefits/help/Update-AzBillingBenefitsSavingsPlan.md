---
external help file:
Module Name: Az.BillingBenefits
online version: https://learn.microsoft.com/powershell/module/az.billingbenefits/update-azbillingbenefitssavingsplan
schema: 2.0.0
---

# Update-AzBillingBenefitsSavingsPlan

## SYNOPSIS
Update savings plan.

## SYNTAX

### UpdateExpanded (Default)
```
Update-AzBillingBenefitsSavingsPlan -Id <String> -OrderId <String>
 [-AppliedScopePropertiesDisplayName <String>] [-AppliedScopePropertiesManagementGroupId <String>]
 [-AppliedScopePropertiesResourceGroupId <String>] [-AppliedScopePropertiesSubscriptionId <String>]
 [-AppliedScopePropertiesTenantId <String>] [-AppliedScopeType <AppliedScopeType>]
 [-BillingPlan <BillingPlan>] [-BillingScopeId <String>] [-CommitmentAmount <Double>]
 [-CommitmentCurrencyCode <String>] [-CommitmentGrain <CommitmentGrain>] [-DisplayName <String>] [-Renew]
 [-RenewPropertiesPurchasePropertiesAppliedScopePropertiesDisplayName <String>]
 [-RenewPropertiesPurchasePropertiesAppliedScopePropertiesManagementGroupId <String>]
 [-RenewPropertiesPurchasePropertiesAppliedScopePropertiesResourceGroupId <String>]
 [-RenewPropertiesPurchasePropertiesAppliedScopePropertiesSubscriptionId <String>]
 [-RenewPropertiesPurchasePropertiesAppliedScopePropertiesTenantId <String>]
 [-RenewPropertiesPurchasePropertiesAppliedScopeType <AppliedScopeType>]
 [-RenewPropertiesPurchasePropertiesDisplayName <String>] [-RenewPropertiesPurchasePropertiesRenew]
 [-SkuName <String>] [-Term <Term>] [-DefaultProfile <PSObject>] [-PassThru] [-Confirm] [-WhatIf]
 [<CommonParameters>]
```

### Update
```
Update-AzBillingBenefitsSavingsPlan -Id <String> -OrderId <String> -Body <ISavingsPlanUpdateRequest>
 [-DefaultProfile <PSObject>] [-PassThru] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-AzBillingBenefitsSavingsPlan -InputObject <IBillingBenefitsIdentity> -Body <ISavingsPlanUpdateRequest>
 [-DefaultProfile <PSObject>] [-PassThru] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-AzBillingBenefitsSavingsPlan -InputObject <IBillingBenefitsIdentity>
 [-AppliedScopePropertiesDisplayName <String>] [-AppliedScopePropertiesManagementGroupId <String>]
 [-AppliedScopePropertiesResourceGroupId <String>] [-AppliedScopePropertiesSubscriptionId <String>]
 [-AppliedScopePropertiesTenantId <String>] [-AppliedScopeType <AppliedScopeType>]
 [-BillingPlan <BillingPlan>] [-BillingScopeId <String>] [-CommitmentAmount <Double>]
 [-CommitmentCurrencyCode <String>] [-CommitmentGrain <CommitmentGrain>] [-DisplayName <String>] [-Renew]
 [-RenewPropertiesPurchasePropertiesAppliedScopePropertiesDisplayName <String>]
 [-RenewPropertiesPurchasePropertiesAppliedScopePropertiesManagementGroupId <String>]
 [-RenewPropertiesPurchasePropertiesAppliedScopePropertiesResourceGroupId <String>]
 [-RenewPropertiesPurchasePropertiesAppliedScopePropertiesSubscriptionId <String>]
 [-RenewPropertiesPurchasePropertiesAppliedScopePropertiesTenantId <String>]
 [-RenewPropertiesPurchasePropertiesAppliedScopeType <AppliedScopeType>]
 [-RenewPropertiesPurchasePropertiesDisplayName <String>] [-RenewPropertiesPurchasePropertiesRenew]
 [-SkuName <String>] [-Term <Term>] [-DefaultProfile <PSObject>] [-PassThru] [-Confirm] [-WhatIf]
 [<CommonParameters>]
```

## DESCRIPTION
Update savings plan.

## EXAMPLES

### Example 1: Update savings plan property value
```powershell
Update-AzBillingBenefitsSavingsPlan -Id "f82fd820-f829-4022-8ba5-e3bf4ffc329b" -OrderId "e0b1f446-5684-4fa6-a0c8-d394368eda11" -DisplayName "NewName"
```

```output
Name        Status    ExpiryDate            PurchaseDate          Term Scope  AppliedScopeDisplayName ProductName          CommitmentAmount CommitmentCurrency
----        ------    ----------            ------------          ---- -----  ----------------------- -----------          ---------------- ------------------
NewName Succeeded 10/25/2025 7:01:05 PM 10/25/2022 6:59:06 PM P3Y  Shared                         Compute_Savings_Plan 0.001            USD
```

Update savings plan property value

## PARAMETERS

### -AppliedScopePropertiesDisplayName
Display name

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppliedScopePropertiesManagementGroupId
Fully-qualified identifier of the management group where the benefit must be applied.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppliedScopePropertiesResourceGroupId
Fully-qualified identifier of the resource group.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppliedScopePropertiesSubscriptionId
Fully-qualified identifier of the subscription.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppliedScopePropertiesTenantId
Tenant ID where the benefit is applied.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppliedScopeType
Type of the Applied Scope.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.BillingBenefits.Support.AppliedScopeType
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BillingPlan
Represents the billing plan in ISO 8601 format.
Required only for monthly billing plans.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.BillingBenefits.Support.BillingPlan
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BillingScopeId
Subscription that will be charged for purchasing the benefit

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Body
Savings plan patch request
To construct, see NOTES section for BODY properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.BillingBenefits.Models.Api20221101.ISavingsPlanUpdateRequest
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -CommitmentAmount
.

```yaml
Type: System.Double
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CommitmentCurrencyCode
The ISO 4217 3-letter currency code for the currency used by this purchase record.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CommitmentGrain
Commitment grain.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.BillingBenefits.Support.CommitmentGrain
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with Azure.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases: AzureRMContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisplayName
Display name

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
ID of the savings plan

```yaml
Type: System.String
Parameter Sets: Update, UpdateExpanded
Aliases: SavingsPlanId

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Identity Parameter
To construct, see NOTES section for INPUTOBJECT properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.BillingBenefits.Models.IBillingBenefitsIdentity
Parameter Sets: UpdateViaIdentity, UpdateViaIdentityExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -OrderId
Order ID of the savings plan

```yaml
Type: System.String
Parameter Sets: Update, UpdateExpanded
Aliases: SavingsPlanOrderId

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Returns true when the command succeeds

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Renew
Setting this to true will automatically purchase a new benefit on the expiration date time.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RenewPropertiesPurchasePropertiesAppliedScopePropertiesDisplayName
Display name

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RenewPropertiesPurchasePropertiesAppliedScopePropertiesManagementGroupId
Fully-qualified identifier of the management group where the benefit must be applied.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RenewPropertiesPurchasePropertiesAppliedScopePropertiesResourceGroupId
Fully-qualified identifier of the resource group.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RenewPropertiesPurchasePropertiesAppliedScopePropertiesSubscriptionId
Fully-qualified identifier of the subscription.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RenewPropertiesPurchasePropertiesAppliedScopePropertiesTenantId
Tenant ID where the benefit is applied.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RenewPropertiesPurchasePropertiesAppliedScopeType
Type of the Applied Scope.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.BillingBenefits.Support.AppliedScopeType
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RenewPropertiesPurchasePropertiesDisplayName
Friendly name of the savings plan

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RenewPropertiesPurchasePropertiesRenew
Setting this to true will automatically purchase a new benefit on the expiration date time.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SkuName
Name of the SKU to be applied

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Term
Represent benefit term in ISO 8601 format.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.BillingBenefits.Support.Term
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.PowerShell.Cmdlets.BillingBenefits.Models.Api20221101.ISavingsPlanUpdateRequest

### Microsoft.Azure.PowerShell.Cmdlets.BillingBenefits.Models.IBillingBenefitsIdentity

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.BillingBenefits.Models.Api20221101.ISavingsPlanModel

## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


`BODY <ISavingsPlanUpdateRequest>`: Savings plan patch request
  - `[AppliedScopePropertiesDisplayName <String>]`: Display name
  - `[AppliedScopePropertiesManagementGroupId <String>]`: Fully-qualified identifier of the management group where the benefit must be applied.
  - `[AppliedScopePropertiesResourceGroupId <String>]`: Fully-qualified identifier of the resource group.
  - `[AppliedScopePropertiesSubscriptionId <String>]`: Fully-qualified identifier of the subscription.
  - `[AppliedScopePropertiesTenantId <String>]`: Tenant ID where the benefit is applied.
  - `[AppliedScopeType <AppliedScopeType?>]`: Type of the Applied Scope.
  - `[BillingPlan <BillingPlan?>]`: Represents the billing plan in ISO 8601 format. Required only for monthly billing plans.
  - `[BillingScopeId <String>]`: Subscription that will be charged for purchasing the benefit
  - `[CommitmentAmount <Double?>]`: 
  - `[CommitmentCurrencyCode <String>]`: The ISO 4217 3-letter currency code for the currency used by this purchase record.
  - `[CommitmentGrain <CommitmentGrain?>]`: Commitment grain.
  - `[DisplayName <String>]`: Display name
  - `[Renew <Boolean?>]`: Setting this to true will automatically purchase a new benefit on the expiration date time.
  - `[RenewPropertiesPurchasePropertiesAppliedScopePropertiesDisplayName <String>]`: Display name
  - `[RenewPropertiesPurchasePropertiesAppliedScopePropertiesManagementGroupId <String>]`: Fully-qualified identifier of the management group where the benefit must be applied.
  - `[RenewPropertiesPurchasePropertiesAppliedScopePropertiesResourceGroupId <String>]`: Fully-qualified identifier of the resource group.
  - `[RenewPropertiesPurchasePropertiesAppliedScopePropertiesSubscriptionId <String>]`: Fully-qualified identifier of the subscription.
  - `[RenewPropertiesPurchasePropertiesAppliedScopePropertiesTenantId <String>]`: Tenant ID where the benefit is applied.
  - `[RenewPropertiesPurchasePropertiesAppliedScopeType <AppliedScopeType?>]`: Type of the Applied Scope.
  - `[RenewPropertiesPurchasePropertiesDisplayName <String>]`: Friendly name of the savings plan
  - `[RenewPropertiesPurchasePropertiesRenew <Boolean?>]`: Setting this to true will automatically purchase a new benefit on the expiration date time.
  - `[SkuName <String>]`: Name of the SKU to be applied
  - `[Term <Term?>]`: Represent benefit term in ISO 8601 format.

`INPUTOBJECT <IBillingBenefitsIdentity>`: Identity Parameter
  - `[Id <String>]`: Resource identity path
  - `[ReservationOrderAliasName <String>]`: Name of the reservation order alias
  - `[SavingsPlanId <String>]`: ID of the savings plan
  - `[SavingsPlanOrderAliasName <String>]`: Name of the savings plan order alias
  - `[SavingsPlanOrderId <String>]`: Order ID of the savings plan

## RELATED LINKS

