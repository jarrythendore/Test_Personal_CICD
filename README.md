} else if (asset.Name.contains('CKYCA Certification') && mapContactWithCKYCAAssets.get(asset.Assignee__c) == null) {
                    mapContactWithCKYCAAssets.put(asset.Assignee__c, new List<Asset>{
                            asset
                    });
                } else if (asset.Name.contains('CKYCA Certification')) {
                    mapContactWithCKYCAAssets.get(asset.Assignee__c).add(asset);
                } 
                else if (asset.Name.contains('CTMA Certification') && mapContactWithCTMAAssets.get(asset.Assignee__c) == null) {  
                    mapContactWithCTMAAssets.put(asset.Assignee__c, new List<Asset> {  
                            asset  
                    });  
                } else if (asset.Name.contains('CTMA Certification')) {  
                    mapContactWithCTMAAssets.get(asset.Assignee__c).add(asset);
                }
  
            }
